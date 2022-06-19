# lectuapi

<p align="center">
  <a>
    <img src="lectulandia.png" height="70px">
  </a>
</p>

## Host

- https://lectuapi.herokuapp.com

## Endpoints

### Libros

Obten todos los libros disponibles.

**GET** https://lectuapi.herokuapp.com/books?limit=2&page=1

```json
{
  "data": [
    {
      "id": "62a903205ce98148ee6a0135",
      "title": "La chica del tren",
      "author": [{ "name": "Paula Hawkins", "slug": "paula-hawkins" }],
      "image": "https://assets.lectulandia.co/b/ab/Paula%20Hawkins/La%20chica%20del%20tren%20(1)/big.jpg",
      "description": "¿Estabas en el tren de las 8.04? ¿Viste algo sospechoso? Rachel, sí. Rachel toma siempre el tren de las 8.04 h. Cada mañana lo mismo: el mismo paisaje, las mismas casas… y la misma parada en la señal roja. Son solo unos segundos, pero le permiten observar a una pareja desayunando tranquilamente en su terraza.Siente que los conoce y se inventa unos nombres para ellos: Jess y Jason. Su vida es perfecta, no como la suya. Pero un día ve algo. Sucede muy deprisa, pero es suficiente. ¿Y si Jess y Jason no son tan felices como ella cree? ¿Y si nada es lo que parece? Tú no la conoces. Ella a ti, sí.",
      "slug": "la-chica-del-tren",
      "genres": [
        { "name": "Intriga", "slug": "intriga" },
        { "name": "Novela", "slug": "novela" },
        { "name": "Policíaco", "slug": "policiaco" }
      ]
    },
    {
      "id": "62a903205ce98148ee6a0136",
      "title": "Ready Player One",
      "author": [{ "name": "Ernest Cline", "slug": "ernest-cline" }],
      "image": "https://assets.lectulandia.co/b/Ernest%20Cline/Ready%20Player%20One%20(4836)/big.jpg",
      "description": "Estamos en el año 2044 y, como el resto de la humanidad, Wade Watts prefiere mil veces el videojuego de OASIS al cada vez más sombrío mundo real. Se afirma que esconde las piezas de un rompecabezas diabólico cuya resolución conduce a una fortuna incalculable. Durante años, millones de humanos han intentado dar con ellas, sin éxito. De repente, Wade logra resolver el primer rompecabezas del premio, y a partir de ese momento debe competir contra miles de jugadores para conseguir el trofeo. La única forma de sobrevivir es ganar. ‘Ready Player One’, el impresionante debut de Ernest Cline, está revolucionando la literatura de género en Estados Unidos. Antes incluso de su publicación, convenció a la Warner Bros., de convertirlo en su próxima gran producción, a agentes y editores de medio mundo de que compraran sus derechos, y cautivó a autores de la talla de Charlaine Harris y Patrick Rothfuss, a quien, según ha confesado, le pareció un libro escrito por él mismo. Desde entonces, esta novela ha seducido a la crítica y ha alcanzado las listas de más vendidos del New York Times y Amazon.",
      "slug": "ready-player-one",
      "genres": [{ "name": "Ciencia ficción", "slug": "ciencia-ficcion" }]
    }
  ],
  "totalPages": 921,
  "currentPage": 1
}
```

### Libro

Obten un libro por su `slug`.

**GET** https://lectuapi.herokuapp.com/books/it

```json
{
  "id": "62a903245ce98148ee6a0139",
  "title": "It",
  "author": [{ "name": "Stephen King", "slug": "stephen-king" }],
  "image": "https://assets.lectulandia.co/b/Stephen%20King/It%20(4930)/big.jpg",
  "description": "¿Quién o qué mutila y mata a los niños de un pequeño pueblo norteamericano? ¿Por qué llega cíclicamente el horror a Derry en forma de un payaso siniestro que va sembrando la destrucción a su paso? Esto es lo que se proponen averiguar los protagonistas de esta novela. Tras veintisiete años de tranquilidad y lejanía una antigua promesa infantil les hace volver al lugar en el que vivieron su infancia y juventud como una terrible pesadilla. Regresan a Derry para enfrentarse con su pasado y enterrar definitivamente la amenaza que los amargó durante su niñez. Saben que pueden morir, pero son conscientes de que no conocerán la paz hasta que aquella cosa sea destruida para siempre. It es una de las novelas más ambiciosas de Stephen King, donde ha logrado perfeccionar de un modo muy personal las claves del género de terror.",
  "slug": "it",
  "genres": [{ "name": "Terror", "slug": "terror" }]
}
```

### Género

Obten los libros por el `slug` del género.

**GET** https://lectuapi.herokuapp.com/genre/terror?limit=10&page=1

### Autor

Obten los libros por el `slug` del autor.

**GET** https://lectuapi.herokuapp.com/author/stephen-king

## Help us

<a href="https://www.buymeacoffee.com/golang4us" target="_blank">
<img src="https://camo.githubusercontent.com/2e6f39f21c4d34ba1a4b01c34d27bb7e9dabb7d5c01fc8a4a2f1a571c36f4d5e/68747470733a2f2f63646e2e6275796d6561636f666665652e636f6d2f627574746f6e732f76322f64656661756c742d79656c6c6f772e706e673f773d33383426713d3735" width="200">
</a>
