# README.md

## Descrição

Este script em Python automatiza o fechamento de chamados via API. Ele lê um arquivo Excel contendo os IDs dos chamados a serem fechados e, para cada ID, envia uma requisição à API correspondente para fechar o chamado no sistema.

## Pré-requisitos

- **Python 3.x** instalado no seu sistema.

### Bibliotecas Python necessárias

O script utiliza as seguintes bibliotecas:

- `requests`
- `pandas`
- `python-dotenv`
- `openpyxl` (necessária para leitura de arquivos Excel)

Você pode instalar todas as dependências executando:

```bash
pip install -r requirements.txt
```
Ou individualmente:
```bash
pip install requests pandas python-dotenv openpyxl
```
Feito isso, configure as variaveis de ambiente da seguinte forma. Abra o CMD e execute os seguintes comandos, atentando-se a subistituir os dados obrigatório:
```bash
# Para módulo de produção:
setx TOKEN_API_IXC_VELOO "seu_token_api_aqui"
setx HOST_IXC_VELOO "seu_host_aqui"

# Para módulo de teste:
setx TOKEN_API_IXC_VELOO_TESTE "seu_token_api_aqui"
setx HOST_IXC_VELOO_TESTE "seu_host_aqui"
```

Com isso, substitua a variável _caminho_arquivo_, para o caminho do seu arquivo, atentando-se para a coluna de id dos chamados está nomeada como 'id_chamado', pois a iteração, referencia-se a coluna _id_chamado_.

Exemplo:
```bash
# Leitura do arquivo Excel para extrair os IDs dos contratos
caminho_arquivo = r"C:\Users\Weslley\Downloads\dados_os_filial18.xlsx"
```