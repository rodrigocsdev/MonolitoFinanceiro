unit MonolitoFinanceiro.Utilitarios;

interface

uses
  Vcl.DBGrids;
type
  TUtilitarios = class
    class function GetID : String;
    class function LikeFind(Pesquisa : string; Grid : TDBGrid) : string;
    class function FormatoMoeda(aValue : Currency) : string;
  end;
implementation

uses
  System.SysUtils;

{ TUtilitarios }

class function TUtilitarios.FormatoMoeda(aValue: Currency): string;
begin
  Result := Format('%m', [aValue]);
end;

class function TUtilitarios.GetID: String;
begin
  Result := TGUID.NewGuid.ToString;
  Result := StringReplace(Result, '{', '', [rfReplaceAll]);
  Result := StringReplace(Result, '}', '', [rfReplaceAll]);
end;

class function TUtilitarios.LikeFind(Pesquisa: string; Grid: TDBGrid): string;
var
  LContador : Integer;
begin
  Result := '';
  if Pesquisa.Trim.IsEmpty then
    exit;
  for LContador := 0 to Pred(Grid.Columns.Count) do
    Result := Result + Grid.Columns.Items[LContador].FieldName +
      ' LIKE ' + QuotedStr('%' + Trim(Pesquisa) + '%') + ' OR ';
  Result := ' AND (' + Copy(Result, 1, Length(Result) - 4) + ')';
end;

end.
