# Getting Started

Die Aufgabe ist es innerhalb von 30 Minuten, eine einfache Spring Boot Applikation zu entwickeln, welche 

1. eine REST API für Personendaten bereitstellt
2. Personen entweder alle oder eine einzelne Person gelesen werden können

## REST Calls

Folgende Requests sollen zum Schluss funktionieren:

### Alle Personen lesen

```http request
GET http://localhost:8080/persons
Accept: application/json
```

### Eine spezifische Person lesen

```http request
GET http://localhost:8080/persons/2
Accept: application/json
```

## Hinweise

- Es braucht keine Datenbank.
- Aufgrund der beschränkten Zeit dürfen (müssen aber keine) JUnit Tests verwendet werden. 
- Die Applikation soll möglichst einfach aufgebaut sein.
- Eine Person verfügt über eine ID, einen Namen und ein Alter. Nachfolgend findet sich eine JSON Representation der Person:

```json
{
  "id": 2,
  "name": "Greta",
  "age": 24
}
```
- Die Spring Boot Applikation kann in der IDE oder auf der Kommandozeile mittels `./gradlew bootRun` gestartet werden.
