# Iniciando projeto

1. criar um ambiente virtual
    python -m venv venv

2. ativar o ambiente virtual
    . venv/bin/activate

3. instalar o django
    pip install django

    <!-- pode ser necessario atualizar o pip " python.exe -m pip install --upgrade pip " -->

# Iniciando o Django
1. criar as configurações base do django
    django-admin startproject projeto .

2. alterar algumas configurações no 

3. [ settings.py ], na variavel TEMPLATES em 'DIRS' : [], adicionar um nome de diretorio que esteja na raiz para servir de templates base no projeto

    EXEMPLO:
        'DIRS': [
            BASE_DIR / 'base_templates'
        ],

4. [ settings.py ], nas variaveis LANGUAGE_CODE e TIME_ZONE alterar para o padrão do Brasil

    LANGUAGE_CODE = 'pt-br'

    TIME_ZONE = 'America/Sao_Paulo'

5. [ settings.py ], Adicionar 2 variaveis referentes aos arquivos static

    STATICFILES_DIRS = (
        BASE_DIR / 'base_statics',
    )

    STATIC_ROOT = BASE_DIR / 'static'  # collectstatic


# Iniciar app

    python manage.py startapp nomeApp

# Outros comandos

. venv/bin/activate
python manage.py runserver

python manage.py makemigrations
python manage.py migrate

python manage.py createsuperuser


# Git