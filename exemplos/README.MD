# Dicionário de Dados do JSON

## tipo
- **Descrição:** Define o tipo do processo.
- **Exemplo:** "Processo Judicial"
    ```json
     {
        "tipo": "Processo Judicial"
     }
    ```

## versao
- **Descrição:** Versão do processo.
- **Exemplo:** "1.00.00"
    ```json
     {
        "versao": "1.00.00"
     }
    ```


## origem
- **Descrição:** Informações sobre a origem do processo.
    - **nome:** Nome da instituição de origem.
    - **url:** URL da instituição de origem.
- **Exemplo:**
    ```json
    {
        "nome": "Tribunal",
        "url": "https://consultapublicapje.tjba.jus.br/pje-web/ConsultaPublica/listView.seam"
    }
    ```

## capa
- **Descrição:** Detalhes sobre a capa do processo.
    - **assunto:** Assunto do processo.
    - **tipoAcao:** Tipo de ação judicial.
    - **classe:** Classe do processo.
    - **dataAjuizamento:** Data de ajuizamento do processo.
    - **magistrado:** Nome do magistrado responsável.
    - **nivelSigilo:** Nível de sigilo do processo.
    - **numeros:**
        - **cliente:** Número do cliente.
        - **cnj:** Número CNJ do processo.
        - **interno:** Número interno do processo.
        - **adicional:** Número adicional do processo.
    - **orgao:**
        - **codigo:** Código do órgão.
        - **instancia:** Instância do órgão.
        - **localidade:** Localidade do órgão.
        - **vara:** Nome da vara.
        - **nome:** Nome do órgão.
        - **uf:** UF do órgão.
- **Exemplo:**
    ```json
    {
        "assunto": "DIREITO CIVIL - Obrigações - Espécies de Contratos - Compra e Venda",
        "tipoAcao": "",
        "classe": "EXECUÇÃO DE TÍTULO EXTRAJUDICIAL (159)",
        "dataAjuizamento": "2019-02-13T00:00:00-03:00",
        "magistrado": "",
        "nivelSigilo": "Público",
        "numeros": {
            "cliente": "",
            "cnj": "8000260-85.2019.8.05.0154",
            "interno": "",
            "adicional": ""
        },
        "orgao": {
            "codigo": "",
            "instancia": "Primeiro Grau",
            "localidade": "LUIS EDUARDO MAGALHÃES",
            "vara": "",
            "nome": "TJBA - Tribunal de Justiça do Estado da Bahia",
            "uf": "BA"
        }
    }
    ```

## dadosComplementares
- **Descrição:** Dados complementares do processo.
    - **tipo:** Tipo de dado complementar.
    - **tipoDado:** Tipo do dado.
    - **data:** Data relacionada ao dado.
    - **valor:** Valor do dado complementar.
- **Exemplo:**
    ```json
    [
        {
            "tipo": "tipoProcesso",
            "tipoDado": "string",
            "data": "",
            "valor": "Processo eletrônico"
        },
        {
            "tipo": "consulta",
            "tipoDado": "string",
            "data": "2019-02-13T00:00:00-03:00",
            "valor": "Consulta PJe Primeiro Grau"
        }
    ]
    ```

## advogados
- **Descrição:** Informações sobre os advogados envolvidos no processo.
    - **documento:**
        - **numero:** Número do documento.
        - **tipo:** Tipo do documento.
        - **uf:** UF do documento.
    - **nome:** Nome do advogado.
    - **oab:** Número da OAB do advogado.
    - **ufOab:** UF da OAB do advogado.
    - **envolvimento:** Envolvimento do advogado no processo.
    - **parte:** Parte representada pelo advogado.
- **Exemplo:**
    ```json
    [
        {
            "documento": {
                "numero": "111.111.111-11",
                "tipo": "CPF",
                "uf": ""
            },
            "nome": "GLORIA OLIVEIRA",
            "oab": "12345",
            "ufOab": "BA",
            "envolvimento": "Polo Ativo",
            "parte": "JOAO ANTONIO"
        }
    ]
    ```

## envolvidos
- **Descrição:** Informações sobre as partes envolvidas no processo.
    - **documento:**
        - **numero:** Número do documento.
        - **tipo:** Tipo do documento.
        - **uf:** UF do documento.
    - **nome:** Nome da parte envolvida.
    - **envolvimento:** Envolvimento da parte no processo.
    - **qualificacao:** Qualificação da parte.
- **Exemplo:**
    ```json
    [
        {
            "documento": {
                "numero": "111.111.111-11",
                "tipo": "CPF",
                "uf": ""
            },
            "nome": "JOAO ANTONIO",
            "envolvimento": "Polo Ativo",
            "qualificacao": "Autor"
        }
    ]
    ```

## movimentacoes
- **Descrição:** Detalhes sobre as movimentações do processo.
    - **data:** Data da movimentação.
    - **texto:** Descrição da movimentação.
    - **documento:** Documento relacionado à movimentação.
    - **id:** ID da movimentação.
    - **prazo:** Prazo relacionado à movimentação.
    - **responsavel:** Responsável pela movimentação.
    - **tipo:** Tipo da movimentação.
- **Exemplo:**
    ```json
    [
        {
            "data": "2019-12-11T00:00:00-03:00",
            "texto": "Conclusos para decisão",
            "documento": "",
            "id": "60d6f438ef50563549655a19bfd68493",
            "prazo": "",
            "responsavel": "",
            "tipo": ""
        }
    ]
    ```

## processosVinculados
- **Descrição:** Detalhes sobre os processos vinculados.
    - **instancia:** Instância do processo vinculado.
    - **numero:** Número do processo vinculado.
    - **orgao:** Órgão relacionado ao processo vinculado.
    - **tipo:** Tipo de vinculação do processo.
- **Exemplo:**
    ```json
    [
        {
            "instancia": "2",
            "numero": "000260-85.2019.8.05.0154/0002",
            "orgao": "TJBA - Tribunal de Justiça do Estado da Bahia",
            "tipo": "Incidente"
        }
    ]
    ```

## schema
- **Descrição:** Esquema do processo.

## documentos
- **Descrição:** Documentos relacionados ao processo.
    - **url:** URL do documento.
    - **nome:** Nome do documento.
    - **tamanho:** Tamanho do documento.
    - **tipo:** Tipo do documento.
    - **mimeType:** Tipo MIME do documento.
    - **md5:** Hash MD5 do documento.
    - **dataValidade:** Data de validade do documento.
    - **dadosComplementares:**
        - **tipo:** Tipo do dado complementar.
        - **tipoDado:** Tipo do dado.
        - **valor:** Valor do dado complementar.
- **Exemplo:**
    ```json
    [
        {
            "url": "https://servidordearquivos.com.br/processos/8000260-85.2019.8.05.0154.pdf",
            "nome": "8000260-85.2019.8.05.0154.pdf",
            "tamanho": "9.8MB",
            "tipo": "pdf",
            "mimeType": "application/pdf",
            "md5": "7e5978ffc68229b16d051499bf27097e",
            "dataValidade": "2024-05-13T00:00:00-03:00",
            "dadosComplementares": [
                {
                    "tipo": "",
                    "tipoDado": "",
                    "valor": ""
                }
            ]
        }
    ]
    ```

## valores
- **Descrição:** Valores relacionados ao processo.
    - **data:** Data relacionada ao valor.
    - **id:** ID do valor.
    - **moeda:** Moeda do valor.
    - **tipo:** Tipo do valor.
    - **valor:** Valor.
- **Exemplo:**
    ```json
    [
        {
            "data": "2019-02-13T00:00:00-03:00",
            "id": "1",
            "moeda": "R$",
            "tipo": "Valor da ação",
            "valor": "1400.00"
        }
    ]
    ```

## classes
- **Descrição:** Classes relacionadas ao processo.
