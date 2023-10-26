object frmPrincipal: TfrmPrincipal
  Left = 0
  Top = 0
  Caption = 'Monolito Financeiro'
  ClientHeight = 417
  ClientWidth = 642
  Color = clBtnFace
  Font.Charset = DEFAULT_CHARSET
  Font.Color = clWindowText
  Font.Height = -16
  Font.Name = 'Tahoma'
  Font.Style = []
  Menu = MainMenu1
  Position = poScreenCenter
  WindowState = wsMaximized
  OnCreate = FormCreate
  TextHeight = 19
  object StatusBar1: TStatusBar
    Left = 0
    Top = 391
    Width = 642
    Height = 26
    Panels = <
      item
        Width = 150
      end
      item
        Width = 300
      end>
  end
  object MainMenu1: TMainMenu
    Left = 496
    Top = 32
    object mnuCadastro: TMenuItem
      Caption = 'Cadastros'
      object mnuUsuarios: TMenuItem
        Caption = 'Usu'#225'rios'
        OnClick = mnuUsuariosClick
      end
    end
    object mnuFinanceiro: TMenuItem
      Caption = 'Financeiro'
      object mnuCaixa: TMenuItem
        Caption = 'Caixa'
        OnClick = mnuCaixaClick
      end
      object mnuContasPagar: TMenuItem
        Caption = 'Contas a Pagar'
        OnClick = mnuContasPagarClick
      end
      object mnuContasReceber: TMenuItem
        Caption = 'Contas a Receber'
        OnClick = mnuContasReceberClick
      end
      object mnuContasReceberConsultar: TMenuItem
        Caption = 'Consultar Contas a Receber'
        OnClick = mnuContasReceberConsultarClick
      end
      object mnuContasPagarConsultar: TMenuItem
        Caption = 'Consultar Contas a Pagar'
        OnClick = mnuContasPagarConsultarClick
      end
    end
    object mnuRelatorios: TMenuItem
      Caption = 'Relat'#243'rios'
      object mnuResumoCaixa: TMenuItem
        Caption = 'Resumo do Caixa'
        OnClick = mnuResumoCaixaClick
      end
      object mnuExtratoCaixa: TMenuItem
        Caption = 'Extrato do Caixa'
        OnClick = mnuExtratoCaixaClick
      end
    end
    object mnuAjuda: TMenuItem
      Caption = 'Ajuda'
    end
  end
  object Timer1: TTimer
    OnTimer = Timer1Timer
    Left = 576
    Top = 320
  end
end
