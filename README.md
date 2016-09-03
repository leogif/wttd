# Eventex

Curso Welcome to the Django.

## Como desenvolver?

Ou siga o passo a passo.

1. Clone o repositório.
2. Crie um virtualenv com Python 3.5
3. Ative o virtualenv.
4. Instale as dependências.
5. Configure a instância com o .env
6. Execute os testes.

```
git clone https://github.com/leogif/wttd.git
cd wttd
python -m venv .wttd
source .wttd/bin/activate # Linux
pip install -r requirements.txt
python contrib/env_gen.py
var=`python contrib/secret_gen.py`
printf '\nSECRET_KEY='$var >> .env
python manage.py test
```