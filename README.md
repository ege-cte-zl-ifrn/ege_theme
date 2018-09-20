# EGE Django Theme

```
pip install ege-django-theme
```

Adicione o aplicativo ao ```settings.py``` na variável de configuração ```INSTALLED_APPS``` antes das aplicações do django:

```
INSTALLED_APPS = 'ege_django_theme',
                 'django.contrib.admin',
                 'django.contrib.auth',
                 ......................
```

Certifique-se de que está setada a variável ```STATIC_URL = '/static/'```.

Em ```urls.py``` inclua a url do Tema:

```
from django.conf.urls import include,
.......

urlpatterns = [
    path('', include('ege_django_theme.urls')),
    ........
```
