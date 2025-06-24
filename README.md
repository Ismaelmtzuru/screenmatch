# 🎬 Screenmatch - Series Search and Management Application

This project combines a **Java Spring Boot** backend and a **web frontend using HTML/JavaScript**, allowing users to search, save, and view series information via the public **OMDb API**. It is designed for learning Java, Spring Data JPA, REST API consumption, and modular frontend development.

---

## 📌 Key Features (Java Backend)

- Data consumption from the OMDb API.
- Conversion of JSON data to Java objects.
- Persistence of series and episodes using Spring Data JPA.
- Console-based user interface with multiple search and filtering options.
- Integration with `SerieRepository` for entity handling and custom queries.

---

## 🧱 Project Structure (Java)

| File/Class           | Description                                                  |
|----------------------|--------------------------------------------------------------|
| `Principal.java`     | Main class with the interactive menu.                        |
| `Serie`, `Episodio`, `DatosSerie`, `DatosTemporadas` | Data models.                           |
| `SerieRepository`    | JPA interface for persistent data management.                |
| `ConsumoAPI`         | Class responsible for consuming data from the OMDb API.      |
| `ConvierteDatos`     | Class to convert JSON responses into Java objects.           |

---

## 🖥️ Console Menu Options

| Option | Functionality                                                                |
|--------|------------------------------------------------------------------------------|
| 1      | Search and save a series from the web (OMDb API)                            |
| 2      | Search for episodes of a saved series                                       |
| 3      | Display all stored series                                                   |
| 4      | Search for a series by title                                                |
| 5      | Show the Top 5 best-rated series                                            |
| 6      | Search for series by genre/category                                         |
| 7      | Filter series by number of seasons and minimum rating                       |
| 8      | Search episodes by name                                                     |
| 9      | Show Top 5 episodes of a specific series                                    |
| 0      | Exit the program                                                            |

---

## 📦 Prerequisites

- Java 17 or higher  
- Spring Boot 3.2+  
- PostgreSQL (or any compatible DB configured in `application.properties`)  
- OMDb API Key (already included in the code)

---

## 🧪 How to Run

```bash
# Clone or download the repository
# Configure your DB connection in application.properties
./mvnw spring-boot:run
```

## 🌐 Web Interface - Frontend HTML/JS
- The project also includes a web frontend that allows users to:
- View new releases and Top 5 series
- Filter series by category (Action, Drama, Comedy, etc.)
- Navigate to series detail pages and view seasons/episodes
- Interact with data served by the backend

