# bling-utils

Utilitários para upload de imagens em lote para AWS S3.

> O módulo de precificação foi movido para um repositório próprio:
> [GabMalta/price_generator](https://github.com/GabMalta/price_generator).

## Instalação via Git

```bash
pip install git+https://github.com/GabMalta/bling_utils.git
```

Para instalar uma branch/tag específica:

```bash
pip install git+https://github.com/GabMalta/bling_utils.git@master
```

## Configuração

Copie `.env.example` para `.env` e preencha as credenciais:

```
AWS_ACCESS_KEY=
AWS_SECRET_KEY=
BUCKET_NAME=
```

## Exemplo rápido

```python
from amazon_s3 import upload_folder_to_s3_parallel

upload_folder_to_s3_parallel("./imagens", "produtos/")
```
