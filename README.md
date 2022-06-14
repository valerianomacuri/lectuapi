# lectuapi

![lectuapi](lectulandia.png)

## Host:

https://lectuapi.herokuapp.com

## Endpoints

### Libros

Obten todos los libros disponibles.

**GET** https://lectuapi.herokuapp.com/books?limit=2&page=1

```json
{
  "data": [
    {
      "id": "62a63218f1aec7797b4487ee",
      "title": "La chica del tren",
      "author": "Paula Hawkins",
      "image": "https://assets.lectulandia.co/b/ab/Paula%20Hawkins/La%20chica%20del%20tren%20(1)/big.jpg",
      "description": "¿Estabas en el tren de las 8.04? ¿Viste algo sospechoso? Rachel, sí. Rachel toma siempre el tren de las 8.04 h. Cada mañana lo mismo: el mismo paisaje, las mismas casas… y la misma parada en la señal roja. Son solo unos segundos, pero le permiten observar a una pareja desayunando tranquilamente en su terraza.Siente que los conoce y se inventa unos nombres para ellos: Jess y Jason. Su vida es perfecta, no como la suya. Pero un día ve algo. Sucede muy deprisa, pero es suficiente. ¿Y si Jess y Jason no son tan felices como ella cree? ¿Y si nada es lo que parece? Tú no la conoces. Ella a ti, sí.",
      "slug": "la-chica-del-tren",
      "genres": ["intriga", "novela", "policiaco"]
    },
    {
      "id": "62a63219f1aec7797b4487ef",
      "title": "Ready Player One",
      "author": "Ernest Cline",
      "image": "https://assets.lectulandia.co/b/Ernest%20Cline/Ready%20Player%20One%20(4836)/big.jpg",
      "slug": "ready-player-one",
      "genres": ["ciencia-ficcion"]
    }
  ],
  "totalPages": 803,
  "currentPage": 1
}
```

### Libro

Obten un libro por su `slug`.

**GET** https://lectuapi.herokuapp.com/books/it

```json
{
  "id": "62a6321bf1aec7797b4487f2",
  "title": "It",
  "author": "Stephen King",
  "image": "https://assets.lectulandia.co/b/Stephen%20King/It%20(4930)/big.jpg",
  "slug": "it",
  "genres": ["terror"]
}
```

### Buscar

Busca un libro

**GET** https://lectuapi.herokuapp.com/search/inteligencia

```json
[
  {
    "id": "62a6347bf1aec7797b448bd9",
    "title": "Maze Runner: Expedientes secretos",
    "author": "James Dashner",
    "image": "https://assets.lectulandia.co/b/ab/James%20Dashner/Maze%20Runner%20Expedientes%20secretos%20(7)/big.jpg",
    "description": "Maze Runner: Expedientes Secretos es una recopilación de documentos clasificados y confidenciales.E-mails entre empleados de CRUEL, memos que debían ser destruidos luego de ser leídos y una selección de los recuerdos borrados de algunos Habitantes componen este original libro escrito por James Dashner e ilustrado por Marcelo Orsi Blanco.Estos archivos secretos ofrecen una mirada única al mundo de Maze Runner y son de lectura obligada para los fans de la saga.Luego de acceder a esta información, cada uno sabrá claramente si CRUEL es bueno. O no…",
    "slug": "maze-runner-expedientes-secretos",
    "genres": ["fantastico", "juvenil", "novela"]
  },
  {
    "id": "62a6345ef1aec7797b448baa",
    "title": "Maze Runner: La cura mortal",
    "author": "James Dashner",
    "image": "https://assets.lectulandia.co/b/ab/James%20Dashner/Maze%20Runner%20La%20cura%20mortal%20(9)/big.jpg",
    "description": "Thomas no se puede confiar en CRUEL. La organización le robó sus recuerdos y lo encerró en el laberinto. Luego lo dejó al borde de la muerte, en el desierto. Y lo separó de los Habitantes, sus únicos amigos. Ahora CRUEL asegura que el tiempo de las mentiras ha terminado. Con toda la información que reunió gracias a las pruebas, está en condiciones de avanzar en la cura de la Llamarada. Pero Thomas debe pasar por la prueba final. ¿Logrará sobrevivir al procedimiento? ¿Será cierto que se terminaron las mentiras? Quizá la verdad sea más terrible aún... una solución letal sin retorno.",
    "slug": "maze-runner-la-cura-mortal",
    "genres": ["fantastico", "juvenil", "novela"]
  },
  {
    "id": "62a63257f1aec7797b44885b",
    "title": "Maze Runner: Correr o morir",
    "author": "James Dashner",
    "image": "https://assets.lectulandia.co/b/ab/James%20Dashner/Maze%20Runner%20Correr%20o%20morir%20(11)/big.jpg",
    "description": "Al despertar dentro de un oscuro elevador en movimiento, lo único que Thomas logra recordar es su nombre. No sabe quién es. Tampoco hacia dónde va. Pero no está solo: cuando la caja llega a su destino, las puertas se abren y se ve rodeado por un grupo de jóvenes. «Bienvenido al Área, Novicio».El Área. Un espacio abierto cercado por muros gigantescos. Al igual que Thomas, ninguno de ellos sabe cómo ha llegado allí. Ni por qué. De lo que están seguros es de que cada mañana las puertas de piedra del laberinto que los rodea se abren y por la noche, se cierran. Y que cada treinta días alguien nuevo es entregado por el elevador.Un hecho altera de forma radical la rutina del lugar: llega una chica, la primera enviada al Área. Y más sorprendente todavía es el mensaje que trae.Thomas será más importante de lo que imagina. Pero para eso deberá descubrir los sombríos secretos guardados en su mente. Por alguna razón, sabe que para lograrlo debe correr. Correr será la clave. O morirá.James Dashner ha urdido un apasionante thriller psicológico y de acción. «Correr o morir» es el primer título de una trilogía que atrapará sin concesiones al lector. Porque cada salida puede convertirse en el pasaje a una verdadera pesadilla…",
    "slug": "maze-runner-correr-o-morir",
    "genres": ["fantastico", "juvenil", "novela"]
  },
  {
    "id": "62a632dbf1aec7797b448942",
    "title": "Blade Runner. ¿Sueñan los androides con ovejas eléctricas?",
    "author": "Philip K. Dick",
    "image": "https://assets.lectulandia.co/b/ab/Philip%20K%20Dick/Blade%20Runner%20Suenan%20los%20androides%20con%20ovejas%20electricas%20(28)/big.jpg",
    "description": "Tras la guerra nuclear, la Tierra ha quedado sometida bajo una gran nube de polvo radioactivo. La gente ha emigrado a otros planetas del sistema y se ha llevado a androides que les asisten. Algunos de estos han escapado de la servidumbre y han vuelto ilegalmente a la Tierra. Y Rick Deckard, cazador de bonificaciones, es uno de los encargados de acabar con ellos. Pero, ¿es justo matar a los humanoides sólo por el hecho de serlo? ¿Cuál es el límite entre la vida artificial y la natural?",
    "slug": "blade-runner-suenan-los-androides-con-ovejas-electricas",
    "genres": ["ciencia-ficcion", "novela"]
  }
]
```
