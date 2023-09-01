# flutter-web-dockerfile

Este archivo debe ser agregar al proyecto actual de Flutter y ejecutar los comando para crear la imagen de Docker necesaria, para usar con Docker Compose o de forma individual. Configuración relacionada con https://github.com/danielnaranjo/go-postgres-docker

### Crear imagen
```
docker build -t flutter-web .
# en caso de haber problema con el cache, usar: docker build --no-cache -t flutter-web .
```

### Probar
```
docker run -d -p 1200:80 --name flutter flutter-web
```

Abre el navegador: http://localhost:1200/
