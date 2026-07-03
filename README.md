# Spring Boot Projects

A monorepo containing multiple independent Spring Boot applications.

## Projects

| Project | Description | Port |
|---|---|---|
| [`todo-api`](./todo-api) | Todo management API | 8080 |
| [`task-api`](./task-api) | Task management API | 8081 |
| [`expense-manager`](./expense-manager) | Expense tracking API | 8082 |

> Update the table above as you add or remove projects.

## Prerequisites

- Java 17+ 
- Maven 3.8+
s
## Getting Started

### Clone the repository

```bash
git clone https://github.com/Khush786Mohammad/spring-boot-projects.git
cd spring-boot-projects
```

### Build a specific project

```bash
cd todo-api
./mvnw clean install -U
```

### Run a specific project

```bash
cd todo-api
./mvnw spring-boot:run
```

Each project runs independently on its own port (see table above). Update `application.properties` in each project if you need to change ports or other settings.

## Project Structure

```
.
├── todo-api/
│   ├── src/
│   ├── pom.xml
│   └── README.md          # project-specific details
├── task-api/
│   ├── src/
│   ├── pom.xml
│   └── README.md
├── expense-manager/
│   ├── src/
│   ├── pom.xml
│   └── README.md
├── .gitignore
└── README.md               # you are here
```

Each sub-project is self-contained with its own `pom.xml` and can be built, run, and tested independently.

## Testing

Run tests for a specific project:
```bash
cd todo-api
./mvnw test
```
