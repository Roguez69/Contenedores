# Servicio de Predicción

Este proyecto es un servicio REST API que simula el uso de un modelo de predicción. El servicio está configurado mediante el uso de contenedores Docker.

## Información del Servicio

El servicio proporciona dos endpoints principales:
- `/`: Muestra una página de bienvenida.
- `/prediccion`: Permite realizar una "predicción" sumando dos números proporcionados.

## Requerimientos

- Docker
- Docker Compose (opcional para facilitar el manejo de contenedores)

## Instalación

1. Clona el repositorio:
    ```bash
    git clone https://github.com/Roguez69/Contenedores.git
    cd Contenedores
    ```

2. Construye el contenedor Docker:
    ```bash
    docker build -t prediction-service .
    ```

3. Ejecuta el contenedor Docker:
    ```bash
    docker run -p 5000:5000 prediction-service
    ```

## Uso (Producción con Ejemplos de cada Endpoint)

### Página de Bienvenida

- **Endpoint:** `/`
- **Método:** GET
- **Descripción:** Muestra una página de bienvenida.

**Ejemplo de Solicitud:**
```bash
curl http://localhost:5000/
