# Gestor de tasques

Aplicació web de gestió de tasques desenvolupada com a **Pràctica 3 (PT3) d'Entorns de desenvolupament**. Permet crear tasques, consultar-ne l'estat, marcar-les com a completades i eliminar-les.

## Tecnologies

- Java 21
- Spring Boot 3.3.5
- Spring MVC i Thymeleaf
- Maven

## Funcionalitats

- Afegir tasques amb una descripció no buida.
- Consultar les tasques pendents i completades.
- Marcar tasques com a completades o eliminar-les.
- Veure un resum del progrés, amb el nombre de tasques i el percentatge completat.

Les tasques es mantenen en memòria; no s'utilitza una base de dades, de manera que les dades es perden en reiniciar l'aplicació.

## Execució

Cal tenir Java 21 instal·lat. Des de l'arrel del projecte, inicia l'aplicació amb el Maven Wrapper:

```bash
./mvnw spring-boot:run
```

Obre [http://localhost:8080](http://localhost:8080) al navegador.

Per executar les proves:

```bash
./mvnw test
```

## Estructura principal

- `src/main/java/org/entdes/todolist/`: aplicació Spring Boot, controlador web, gestor i model de tasques.
- `src/main/resources/templates/`: vistes Thymeleaf.
- `src/main/resources/static/`: fulls d'estil.
- `src/test/java/org/entdes/todolist/`: proves de l'aplicació i del controlador.
