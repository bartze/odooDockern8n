# Odoo Docker n8n

Este proyecto configura Odoo utilizando Docker, facilitando la implementación y gestión de un entorno Odoo.

## Estructura del Proyecto

```plaintext
odooDockern8n/
├── dev_addons/
│   └── manage/
│       ├── controllers/
│       ├── demo/
│       ├── models/
│       ├── security/
│       ├── views/
│       ├── __init__.py
│       └── __manifest__.py
├── logs/
├── docker-compose.yaml
└── odoo.conf
```
## Prerrequisitos
    - Docker
    - Docker compose

## configuración

1. Clonar el Repositorio
```
git clone https://github.com/bartze/odooDockern8n.git
cd odooDockern8n
```
2. Configurar las Variables de Entorno
Crear un archivo .env en la raiz del proyecto con las siguientes variables:
POSTGRES_USER=odoo
POSTGRES_PASSWORD=odoo
POSTGRES_DB=postgres
HOST=db
USER=odoo
PASSWORD=odoo

3. Iniciar los Servicios
```
docker-compose up -d
```

4. Acceder a Odoo
http://localhost:8069

## Uso

### Añadir Módulos
Añadir nuevos módulos a la carpeta `dev_addons`.

## Contribución
Las contribuciones son bienvenidas. Por favor, siga los pasos a continuación para contribuir:

1. Haga un fork del proyecto.
2. Cree una nueva rama (`git checkout -b feature/nueva-feature`).
3. Realice sus cambios y haga un commit (`git commit -am 'Añadir nueva feature'`).
4. Haga push a la rama (`git push origin feature/nueva-feature`).
5. Cree un nuevo Pull Request.

## Licencia
Este proyecto está licenciado bajo la Licencia MIT.

