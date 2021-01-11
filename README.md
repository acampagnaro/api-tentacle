SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
ALTER PROCEDURE [dbo].[SP_CLID060_Insert]
                                (
                                  @tbCodigo int output,
                                  @tbNome varchar(50),
                                  @tbDtNasc datetime,
                                  @tbSexo varchar(1),
                                  @tbEndereco varchar(60),
                                  @tbBairro varchar(50),
                                  @tbCidade varchar(255),
                                  @tbEstado varchar(2),
                                  @tbCEP varchar(8),
                                  @tbFoneRes varchar(20),
                                  @tbFoneCom varchar(20),
                                  @tbCelular varchar(40),
                                  @tbEmail varchar(60),
                                  @tbEstadoCivil int = 0,
                                  @tbProfissao int,
                                  @tbRg varchar(20),
                                  @tbCPF varchar(20),
                                  @tbCor varchar(20),
                                  @tbNacionalidade varchar(50),
                                  @tbNaturalidade varchar(50),
                                  @tbNomemae varchar(50),
                                  @tbNomePai varchar(50),
                                  @tbEndResp varchar(50),
                                  @tbFoneResp varchar(20),
                                  @tbIndicador varchar(50),
                                  @tbCodConv int,
                                  @tbCodMedico int,
                                  @tbAuditoria text,
                                  @tbCodRaca int = 0,
                                  @tbInternetSenha varchar(8),
                                  @tbInternetLogado bit,
                                  @tbVinculo bigint,
                                  @tbDataCadastro datetime,
                                  @tbPlano varchar(40),
                                  @tbCPFPai numeric(9),
                                  @tbCPFMae numeric(9),
                                  @tbFoneResCompl varchar(20),
                                  @tbFoneComCompl varchar(20),
                                  @tbCelularCompl varchar(40),
                                  @tbFichaPai int
                                )
AS
SET @tbCodigo = (SELECT MAX(tbSequencia) + 1 FROM clinic.dbo.Sequencia WHERE tbCampo = 'clid060');
INSERT INTO CLID060
               (
                 tbCodigo ,
                 tbNome ,
                 tbDtNasc ,
                 tbSexo ,
                 tbEndereco ,
                 tbBairro ,
                 tbCidade ,
                 tbEstado ,
                 tbCEP ,
                 tbFoneRes ,
                 tbFoneCom ,
                 tbCelular ,
                 tbEmail ,
                 tbEstadoCivil ,
                 tbProfissao ,
                 tbRg ,
                 tbCPF ,
                 tbCor ,
                 tbNacionalidade ,
                 tbNaturalidade ,
                 tbNomemae ,
                 tbNomePai ,
                 tbEndResp ,
                 tbFoneResp ,
                 tbIndicador ,
                 tbCodConv ,
                 tbCodMedico ,
                 tbAuditoria ,
                 tbCodRaca ,
                 tbInternetSenha ,
                 tbInternetLogado ,
                 tbVinculo,
                 tbDataCadastro,
                 tbPlano,
                 tbCPFPai,
                 tbCPFMae,
                 tbFoneResCompl,
                 tbFoneComCompl,
                 tbCelularCompl,
                 tbFichaPai
               )
            Values
               (
                 @tbCodigo ,
                 @tbNome ,
                 @tbDtNasc ,
                 @tbSexo ,
                 @tbEndereco ,
                 @tbBairro ,
                 @tbCidade ,
                 @tbEstado ,
                 @tbCEP ,
                 @tbFoneRes ,
                 @tbFoneCom ,
                 @tbCelular ,
                 @tbEmail ,
                 @tbEstadoCivil,
                 @tbProfissao,
                 @tbRg ,
                 @tbCPF ,
                 @tbCor ,
                 @tbNacionalidade ,
                 @tbNaturalidade ,
                 @tbNomemae ,
                 @tbNomePai ,
                 @tbEndResp ,
                 @tbFoneResp ,
                 @tbIndicador ,
                 @tbCodConv ,
                 @tbCodMedico ,
                 @tbAuditoria ,
                 @tbCodRaca,
                 @tbInternetSenha ,
                 @tbInternetLogado ,
                 @tbVinculo,
                 @tbDataCadastro,
                 @tbPlano,
                 @tbCPFPai,
                 @tbCPFMae,
                 @tbFoneResCompl,
                 @tbFoneComCompl,
                 @tbCelularCompl,
                 @tbFichaPai
               )
-- insert into clinic.dbo.clid060t (tbCodigo) values (@tbCodigo)
update clinic.dbo.Sequencia set tbSequencia = @tbCodigo where tbCampo = 'clid060';
return @tbCodigo
GO




# Bem vindo a API-TENTACLE!


![enter image description here](https://storage.googleapis.com/spitzer-io/img/Spitzer%20Fundo%20Transparente%20aplica%C3%A7%C3%A3o%20em%20PANTONE%20294%20C%20MODELO%202%20%281%29.png)

# Releases

<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/acampagnaro/api-tentacle">

# Feature
Version of integration with **[Risc Sistemas em Saúde Sistemas](https://clinic.med.br)**
