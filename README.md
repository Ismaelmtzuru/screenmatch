# Screenmatch - Aplicación de Búsqueda y Gestión de Series

Este proyecto Java es una aplicación de consola basada en Spring Boot que permite buscar, guardar y consultar información sobre series utilizando la API pública de [OMDb](https://www.omdbapi.com/). Está orientada al aprendizaje de Java, Spring Data JPA y consumo de APIs REST.

## 📌 Características principales

- Consumo de datos desde la API de OMDb.
- Conversión de datos JSON a objetos Java.
- Persistencia de series y episodios en base de datos mediante Spring Data JPA.
- Interfaz de usuario por consola con múltiples opciones de búsqueda y filtrado.
- Integración con `SerieRepository` para manejo de entidades y consultas personalizadas.

## 🧱 Estructura del proyecto

- `Principal.java`: clase principal con el menú interactivo.
- `Serie`, `Episodio`, `DatosSerie`, `DatosTemporadas`: modelos de datos.
- `SerieRepository`: interfaz JPA para la gestión de datos persistentes.
- `ConsumoAPI`: clase encargada de consumir datos desde OMDb API.
- `ConvierteDatos`: clase que convierte respuestas JSON en objetos Java.

## 🖥️ Menú de opciones

| Opción | Funcionalidad |
|--------|---------------|
| `1` | Buscar y guardar una serie desde la web (OMDb API) |
| `2` | Buscar episodios de una serie guardada |
| `3` | Mostrar todas las series almacenadas |
| `4` | Buscar una serie por título |
| `5` | Mostrar el Top 5 de mejores series según evaluación |
| `6` | Buscar series por género/categoría |
| `7` | Filtrar series por cantidad de temporadas y evaluación mínima |
| `8` | Buscar episodios por nombre |
| `9` | Mostrar Top 5 episodios de una serie específica |
| `0` | Salir del programa |

## 📦 Requisitos previos

- Java 17 o superior
- Spring Boot 3.2+
- PostgreSQL o cualquier base de datos compatible configurada en `application.properties`
- OMDb API Key (ya incluida en el código)

## 🧪 Ejecución del proyecto

1. Clona o descarga el repositorio.
2. Configura tu conexión a base de datos en `application.properties`.
3. Ejecuta la aplicación desde tu IDE o desde terminal con:

```bash
./mvnw spring-boot:run
