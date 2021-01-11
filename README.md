SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO

ALTER PROCEDURE [dbo].[SP_CLID060T_Insert]
                                (
                                  @tbCodigo int,
                                  @tbProcedencia varchar(50),
                                  @tbAcompanhante varchar(50),
                                  @tbProfResp int,
                                  @tbRamoParent varchar(50),
                                  @tbUltlaudo int,

                                  @tbUltImpresso int,
                                  @tbTratamento bit,
                                  @tbCampoGene2 varchar(50),
                                  @tbPacienteInativo bit,
                                  @tbSequencia int,
                                  @tbValCarteira datetime,
                                  @tbObservacao text,
                                  @tbAlerta text,
                                  @tbMatricula varchar(20),

                                  @tbPatologia int,
                                  @tbCampoGene1 int,
                                  @tbDataAlter datetime,
                                  @tbPlano varchar(40),
                                  @tbRegionalUnidade int,
                                  @tbCondAlta smallint,
                                  @tbCondAltaData smalldatetime,
                                  @tbCondAltaResp int,
                                  @tbTipoResp tinyint,
                                  @tbEnvMalaDireta bit,

                                  @tbTipoSangue varchar(5),
                                  @tbSorologia varchar(20),
                                  @tbDescendencia varchar(30),
                                  @tbCorOlhos varchar(20),
                                  @tbPeso decimal(18,2),
                                  @tbAltura decimal(18,2),
                                  @tbCNS decimal(15,0),
                                  @tbOlimpo bit
                                )
AS

INSERT INTO CLID060T
               (
                 tbCodigo ,
                 tbProcedencia ,
                 tbAcompanhante ,
                 tbProfResp ,
                 tbRamoParent ,
                 tbUltlaudo ,
                 tbUltImpresso ,
                 tbTratamento ,
                 tbCampoGene2 ,
                 tbPacienteInativo ,

                 tbSequencia ,
                 tbValCarteira ,
                 tbObservacao ,
                 tbAlerta ,
                 tbMatricula ,
                 tbPatologia ,
                 tbCampoGene1 ,
                 tbDataAlter ,
                 tbPlano ,
                 tbRegionalUnidade ,
                 tbCondAlta ,
                 tbCondAltaData ,
                 tbCondAltaResp ,
                 tbTipoResp ,

                 tbEnvMalaDireta,
                 tbTipoSangue,
                 tbSorologia,
                 tbDescendencia,
                 tbCorOlhos,
                 tbPeso,
                 tbAltura,
                 tbCNS,

                 tbOlimpo
               )
            Values
               (
                 @tbCodigo ,
                 @tbProcedencia ,
                 @tbAcompanhante ,
                 @tbProfResp ,
                 @tbRamoParent ,
                 @tbUltlaudo ,
                 @tbUltImpresso ,
                 @tbTratamento ,
                 @tbCampoGene2 ,

                 @tbPacienteInativo ,
                 @tbSequencia ,
                 @tbValCarteira ,
                 @tbObservacao ,
                 @tbAlerta ,
                 @tbMatricula ,
                 @tbPatologia ,
                 @tbCampoGene1 ,
                 @tbDataAlter ,
                 @tbPlano ,
                 @tbRegionalUnidade ,

                 @tbCondAlta ,
                 @tbCondAltaData ,
                 @tbCondAltaResp ,
                 @tbTipoResp ,
                 @tbEnvMalaDireta,
                 @tbTipoSangue,
                 @tbSorologia,
                 @tbDescendencia,
                 @tbCorOlhos,
                 @tbPeso,
                 @tbAltura,
                 @tbCNS,
                 @tbOlimpo
               );

GO




# Bem vindo a API-TENTACLE!


![enter image description here](https://storage.googleapis.com/spitzer-io/img/Spitzer%20Fundo%20Transparente%20aplica%C3%A7%C3%A3o%20em%20PANTONE%20294%20C%20MODELO%202%20%281%29.png)

# Releases

<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/acampagnaro/api-tentacle">

# Feature
Version of integration with **[Risc Sistemas em Saúde Sistemas](https://clinic.med.br)**
