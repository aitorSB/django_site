# DJANGO

## Inicialización del proyecto

> $ django-admin startproject Proyecto1

> $ python manage.py migrate

## Iniciar servidor

> $ python manage.py runserver

## Creación de la web

* Crear fichero views.py
* Importart from django.http import HttpResponse
* Función vista que recibe request
```py
def saludo(request):
    return HttpResponse('Hola mundo!')
```
* Enlazar url con la vista que hemos creado.
    * Fichero urls.py agregar path('saludo/', saludo)
    * Importamos función - módulo: from Proyecto1.views import saludo
