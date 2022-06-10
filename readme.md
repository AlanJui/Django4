# 《專案指引》

## 設定 venv

```sh
pyenv virtualenv 3.10.0 django-4.0
```

```
cd ~/workspace/django
mkdir dj4-001 && cd $_
```

```
pyenv local django-4.0
~/.pyenv/versions/3.10.0/envs/django-4.0/bin/python3.10 -m pip install pip --upgrade
pip install pynvim
```

:checkhealth 驗證 Neovim 已能正常運作。

```
python -m pip install Django
python -m django --version
```

```
django-admin startproject mysite .
```

# 設置專案所需設定檔

- .pyrightconfig.json
- .pylintrc
- .flake8
- .prettierrc.json

## Python Lint

### 設定檔

django-settings-module=<mysite>.settings


### 執行檔

```
pip install pylint-django
```

```
pip install flake8
```

```
pip install django-stubs
```

mypy.ini
```
[mypy]
plugins =
    mypy_django_plugin.main

[mypy.plugins.django-stubs]
django_settings_module = "myproject.settings"
```

## Formatting

```
pip install flake8
pip install autopep8
pip install isort
pip install djlint
pip install djhtml
```


##

```
pip freeze > requirements.txt
```


```
pip install -r requirements.txt
```
