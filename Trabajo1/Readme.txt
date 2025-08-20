Trabajo1/
│
├── ProyectoTrabajo1/ 
│ ├── init.py
│ ├── asgi.py
│ ├── settings.py
│ ├── urls.py
│ └── wsgi.py
│
├── AppTrabajo1/ 
│ ├── migrations/
│ │ └── init.py
│ ├── static/ 
│ │ └── AppTrabajo1/
│ │ └── style.css
│ ├── templates/ 
│ │ └── AppTrabajo1/
│ │ ├── home.html
│ │ └── about.html
│ ├── init.py
│ ├── admin.py
│ ├── apps.py
│ ├── models.py
│ ├── tests.py
│ ├── urls.py
│ └── views.py
│
├── db.sqlite3 
├── manage.py
├── Readme.py
└── requirements.txt

Este proyecto es un ejemplo de aplicación Django con una app llamada AppTrabajo1, que sirve para demostrar el uso de templates, vistas, URLs.

Cuenta con dos páginas principales: Home y About, con navegación entre ellas.


Instalación y ejecución

Descargar el repositorio y entrar en la carpeta "Trabajo1":

cd Trabajo1

Crear y activar el ambiente virtual:

python -m venv .venv (Windows)
python3 -m venv .venv (Linux/Mac)

Activar el ambiente virtual (Windows PowerShell):
..venv\Scripts\Activate.ps1
Si falla la activación por políticas:
Set-ExecutionPolicy -Scope Process -ExecutionPolicy RemoteSigned
..venv\Scripts\Activate.ps1

Linux/Mac:
source .venv/bin/activate

Instalar dependencias:

pip install -r requirements.txt

Preparar la base de datos:

python manage.py migrate

Ejecutar el servidor:

python manage.py runserver

Abrir en el navegador:

Home: http://127.0.0.1:8000/home

About: http://127.0.0.1:8000/home/about