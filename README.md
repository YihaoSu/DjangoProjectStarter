# Django Project Starter

## 專案目錄結構
為了讓專案更為結構化且符合實務， 此專案的目錄結構採用Django專案範本產生器[Cookiecutter Django](https://github.com/pydanny/cookiecutter-django)及[Two Scoops of Django 1.11](https://www.twoscoopspress.com/products/two-scoops-of-django-1-11)一書所偏好的project layout， 而非Django project預設的目錄結構。 專案根目錄[bochweb/](https://github.com/bohachu/bochweb)包含以下子目錄及檔案:

* [config/](https://github.com/YihaoSu/DjangoProjectStarter/tree/master/config)目錄: 包含[settings/](https://github.com/YihaoSu/DjangoProjectStarter/tree/master/config/settings)目錄、[URL設定檔](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/config/urls.py)及[WSGI設定檔](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/config/wsgi.py)。 [settings/](https://github.com/YihaoSu/DjangoProjectStarter/tree/master/config/settings)目錄中又包含用以進行本地端開發 ([local.py](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/config/settings/local.py)) 及正式上線([production.py](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/config/settings/production.py))等不同狀況時的設定檔, 這兩個檔都繼承自基本設定檔[base.py](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/config/settings/base.py)。 

* [ starter/](https://github.com/YihaoSu/DjangoProjectStarter/tree/master/starter)目錄: 包含此專案中司職不同功能的[apps](https://docs.djangoproject.com/en/2.2/ref/applications/)及其所屬的[templates](https://docs.djangoproject.com/en/2.2/ref/templates/)和[static files](https://docs.djangoproject.com/en/2.2/howto/static-files/)。

* [requirements/](https://github.com/YihaoSu/DjangoProjectStarter/tree/master/requirements)目錄: 包含用以進行本地端開發 ([local.txt](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/requirements/local.txt)) 及正式上線([production.txt](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/requirements/production.txt))等不同狀況時的Python套件需求, 這三個檔都繼承自基本套件需求檔[base.txt](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/requirements/base.txt)。 

* [README.md](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/README.md): 此專案GitHub repository的主說明文件。

* [.gitignore](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/.gitignore): 包含git commit時不需要版本控制而要忽略的檔案列表及規則。

* [manage.py](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/manage.py)

* [dot_env_file_template](https://github.com/YihaoSu/DjangoProjectStarter/blob/master/dot_env_file_template): 環境變數.env檔模版，請依據自己的開發環境修改、擴展檔案中的設定(資料庫帳密等等)，並更名為.env ，為了安全性請務必更改模版中的設定值，且不要將本地端/正式機中的.env檔上傳到GitHub。
