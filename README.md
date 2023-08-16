# Co-coro-corre
Juego de scape room de una gallina intentando resolver los problemas
{
  "nombre": "Co coro corre",
  "descripcion": "Eres un valiente pollo que busca escapar de la granja antes de que sea demasiado tarde.",
  "habitacionInicial": "corral",
  "habitaciones": {
    "corral": {
      "nombre": "Corral",
      "descripcion": "Un corral con altas vallas de madera y un camino que lleva a otras áreas.",
      "objetos": [
        {
          "nombre": "Piedra",
          "descripcion": "Una piedra pequeña y redonda que podría ser útil."
        },
        {
          "nombre": "Comedero",
          "descripcion": "Un comedero lleno de granos de maíz.",
          "interacciones": [
            {
              "accion": "buscar",
              "descripcion": "Rebuscas en el comedero y encuentras una llave."
            }
          ]
        }
      ],
      "conexiones": [
        {
          "direccion": "norte",
          "habitacionDestino": "granero"
        },
        {
          "direccion": "este",
          "habitacionDestino": "casa"
        }
      ],
      "pistasGenerales": [
        "Las vallas parecen altas, pero tal vez haya una manera de escalarlas.",
        "El granero y la casa podrían ser buenos lugares para buscar pistas y objetos."
      ]
    },
    "granero": {
      "nombre": "Granero",
      "descripcion": "Un granero oscuro con montones de heno y herramientas agrícolas.",
      "objetos": [
        {
          "nombre": "Horquilla",
          "descripcion": "Una horquilla afilada que podría ser útil para abrir algo."
        },
        {
          "nombre": "Caja",
          "descripcion": "Una caja cerrada con un candado.",
          "interacciones": [
            {
              "accion": "abrir",
              "requiere": "llave",
              "descripcion": "Usas la llave que encontraste en el corral para abrir la caja y encuentras una cuerda."
            }
          ]
        }
      ],
      "conexiones": [
        {
          "direccion": "sur",
          "habitacionDestino": "corral"
        }
      ],
      "pistasGenerales": [
        "La horquilla podría ser útil para abrir algo que esté cerrado con llave.",
        "Tal vez puedas usar la cuerda para crear una herramienta improvisada."
      ]
    },
    "casa": {
      "nombre": "Casa",
      "descripcion": "Una casa rústica con una puerta principal y ventanas con cortinas.",
      "objetos": [
        {
          "nombre": "Huevo",
          "descripcion": "Un huevo fresco y listo para ser comido."
        }
      ],
      "conexiones": [
        {
          "direccion": "oeste",
          "habitacionDestino": "corral"
        }
      ],
      "pistasGenerales": [
        "Puede que encuentres algo útil dentro de la casa.",
        "Explora las habitaciones para ver si hay pistas que te ayuden a escapar."
      ]
    }
  }
}
