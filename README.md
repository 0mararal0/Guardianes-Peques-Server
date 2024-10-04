# Guardianes & Peques

Este repositorio es un [json-server](https://github.com/0mararal0/Guardianes-Peques-Server) creado para introducir datos en la App de React.

#### [Client Repo here](https://github.com/0mararal0/Guardianes-Peques-Server)

# Estructura Server

## Colecciones

### Guardian

```javascript
    {
      "nombre": "",
      "apellidos": "",
      "localidad": "",
      "provincia": "",
      "nacimiento": "",
      "telefono": "",
      "email": "",
      "foto": "",
      "numeroNiños": "",
      "edadesSeleccionadas": {
        "bebe": true,
        "pequeño": true,
        "prescolar": true,
        "escolar": true,
        "adolescente": true
      },
      "serviciosSeleccionados": {
        "cocinar": true,
        "recogida": true,
        "tareas": true,
        "actividades": true,
        "dormir": true
      },
      "diasSemana": {
        "L": true,
        "M": true,
        "X": true,
        "J": true,
        "V": true,
        "S": true,
        "D": true
      },
      "horaInicio": "",
      "horaFin": "",
      "tarifa": 0,
      "comentario": "",
      "id": ""
    },
```

### Client

```javascript
 {
      "niños": "",
      "edadNiño": {
        "bebe": true,
        "pequeño": false,
        "prescolar": false,
        "escolar": false,
        "adolescente": false
      },
      "tareas": {
        "cocinar": true,
        "recogida": false,
        "tareas": false,
        "actividades": false,
        "dormir": false,
        "deberes": false,
        "baño": false
      },
      "reservationWeek": {
        "L": false,
        "M": false,
        "X": false,
        "J": false,
        "V": false,
        "S": true,
        "D": false
      },
      "reservationDay": "",
      "reservationHour": "",
      "reservationTime": "",
      "nombre": "",
      "apellidos": "",
      "email": "",
      "direcion": "",
      "piso": "",
      "letra": "",
      "zip": "",
      "ciudad": "",
      "poblacion": "",
      "telefono": "",
      "guardianId": "",
      "id": ""
    }
```

## Used API Endpoints in the App

| HTTP Method | URL                       | Request Body     | Description                                                                   |
| ----------- | ------------------------- | ---------------- | ----------------------------------------------------------------------------- |
| GET         | `/guardian`               |                  | Ver todos los Guardianes                                                      |
| GET         | `/guardian/:guardianId`   | {id}             | Ver Guardian con ese ID                                                       |
| POST        | `/guardian`               | {data guardian}  | Genera un nuevo Guardian                                                      |
| PUT         | `/guardian/:guardianId`   | {id}             | Modifica la data de un Guardian concreto                                      |
| DELETE      | `/guardian/:guardianId`   | {id}             | Elimina la data de un Guardian concreto                                       |
| GET         | `/guardian?_embed=client` |                  | Ver todos los Guardianes con sus clientes asociados                           |
| POST        | `/client`                 | { data cliente } | Genera una reserva con la data del cliente relacionado a un ID de un Guardian |
| DELETE      | `/client/:id`             | { id }           | Elimina toda la reserva de un cliente en concreto                             |

## Links

### Collaborators

[Developer 1 Miguel Ponte](https://github.com/Miguelitoo2421)

[Developer 2 Alberto Marcos](https://github.com/0mararal0)

### Project

[Repository Link Client](https://github.com/0mararal0/Guardianes-Peques-Client)

[Repository Link Server](https://github.com/0mararal0/Guardianes-Peques-Server)

[Deploy Link](https://guardianesypeques.netlify.app/)

### Slides

[Slides Link](https://guardianesypeques.netlify.app/)
