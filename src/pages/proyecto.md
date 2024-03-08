---
layout: '../../layouts/TopicLayout.astro'
title: 'Proyecto de evaluación'
---

Para la evaluación del curso se realizará un proyecto consiste en una aplicación web clon de Instagram. La aplicación debe tener las siguientes características:

- **Página de login y registro**
  - Debe permitir registrarse con correo y contraseña
  - Sería ideal que al registrarse se pueda agregar una foto de perfil y añadir un nombre de usuario (ver [Bonus: Editar información de usuario](/content/1_6))
- **Página de inicio con las publicaciones de los usuarios**
  - Se debe poder dar like a las publicaciones
  - Se debe poder ver la cantidad de likes que tiene una publicación
  - Se pueden mostrar comentarios y agregar comentarios a las publicaciones (opcional)
- **Página para agregar una nueva publicación**.
  - Debe permitir subir una imagen/insertar una URL
  - Debe permitir agregar una descripción
  - Debe permitir publicar la publicación
- **Página de perfil de usuario con la información del usuario y sus publicaciones**
  - Debe mostrar la foto de perfil, el nombre de usuario y la cantidad de publicaciones
  - Debe mostrar las publicaciones del usuario
  - Al hacer clic en una publicación debe llevarlo a la página de detalle de la publicación
- **Página de detalle de una publicación**
  - Debe mostrar la imagen, el nombre del usuario, la descripción y los comentarios
  - Debe permitir dar like a la publicación
  - Debe permitir poder eliminar la publicación si el usuario es el autor
  - Debe poder llevarlo a la página para editar la publicación si el usuario es el autor
  - Se pueden mostrar comentarios y agregar comentarios a las publicaciones (opcional)
- **Página de edición de una publicación**
  - Debe permitir editar la descripción y la imagen de la publicación
   
Como sugerencia para la estructura de la base de datos, se puede usar la siguiente:

```yaml
posts/: Colección
    - <postId>: Documento
        - userId: string
        - userName: string
        - imageUrl: string
        - description: string
        - likes: number
        - comments/: Colección (opcional)
            - <commentId>: Documento
                - userId: string
                - userName: string
                - text: string
```

El Figma que se mostró en clase puede ser encontrado aquí, con las funcionalidades requeridas y diseños sugeridos: [https://www.figma.com/file/DjIVhG9SM8cE8jNFgv5SEY/Proyecto-de-Vue?type=design&node-id=0%3A1&mode=design&t=9gEy7UMQy5ZLpc4J-1](https://www.figma.com/file/DjIVhG9SM8cE8jNFgv5SEY/Proyecto-de-Vue?type=design&node-id=0%3A1&mode=design&t=9gEy7UMQy5ZLpc4J-1).

El formulario para entregar su proyecto será agregado el jueves.
