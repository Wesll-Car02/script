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
