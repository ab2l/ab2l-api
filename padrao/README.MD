# Dicionário de Dados do JSON

## tipo
- **Descrição:** Define o tipo do processo, que pode ser um processo Judicial ou um processo Administrativo.
- **Exemplo:** "Processo Judicial"
    ```json
     {
        "tipo": "string"
     }
    ```

## versao
- **Descrição:** Versão do processo.
- **Exemplo:** "1.00.00"
    ```json
     {
        "versao": "string"
     }
    ```

## origem
- **Descrição:** Informações sobre a origem do processo.
    - **nome:** Nome da instituição de origem.
    - **url:** URL da instituição de origem.
- **Exemplo:**
    ```json
    {
        "nome": "string",
        "url": "string"
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
        "assunto": "string",
        "tipoAcao": "string",
        "classe": "string",
        "dataAjuizamento": "string",
        "magistrado": "string",
        "nivelSigilo": "string",
        "numeros": {
            "cliente": "string",
            "cnj": "string",
            "interno": "string",
            "adicional": "string"
        },
        "orgao": {
            "codigo": "string",
            "instancia": "string",
            "localidade": "string",
            "vara": "string",
            "nome": "string",
            "uf": "string"
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
            "tipo": "string",
            "tipoDado": "string",
            "data": "string",
            "valor": "string"
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
                "numero": "string",
                "tipo": "string",
                "uf": "string"
            },
            "nome": "string",
            "oab": "string",
            "ufOab": "string",
            "envolvimento": "string",
            "parte": "string"
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
                "numero": "string",
                "tipo": "string",
                "uf": "string"
            },
            "nome": "string",
            "envolvimento": "string",
            "qualificacao": "string"
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
            "data": "string",
            "texto": "string",
            "documento": "string",
            "id": "string",
            "prazo": "string",
            "responsavel": "string",
            "tipo": "string"
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
            "instancia": "string",
            "numero": "string",
            "orgao": "string",
            "tipo": "string"
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
            "url": "string",
            "nome": "string",
            "tamanho": "string",
            "tipo": "string",
            "mimeType": "string",
            "md5": "string",
            "dataValidade": "string",
            "dadosComplementares": [
                {
                    "tipo": "string",
                    "tipoDado": "string",
                    "valor": "string"
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
            "data": "string",
            "id": "string",
            "moeda": "string",
            "tipo": "string",
            "valor": "string"
        }
    ]
    ```

## classes
- **Descrição:** Classes relacionadas ao processo.
    - **data:** Data relacionada à modificação.
    - **classe:** .
    - **motivoAlteracao:** .    
- **Exemplo:**
    ```json
    [
        {
            "data": "",
            "classe": "",
            "motivoAlteracao": ""
        }
    ]
    ```
