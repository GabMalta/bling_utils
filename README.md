# bling-utils

Utilitários para cálculo de preço e upload de imagens para AWS S3.

## Instalação via Git

```bash
pip install git+https://github.com/<usuario>/<repositorio>.git
```

Para instalar uma branch/tag específica:

```bash
pip install git+https://github.com/<usuario>/<repositorio>.git@main
```

## Módulos

- `price_generator`: funções de cálculo de custo e preço.
- `amazon_s3`: funções para upload de imagens em lote para S3.

## Exemplo rápido

```python
from price_generator import calculate_price

preco, custo = calculate_price(cost_price=20.0, multiplier=1.5, profit_margin=20)
print(preco, custo)
```
