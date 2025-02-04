<p align="center"><a href="https://github.com/javiidoce/tfgDam" target="_blank"><img src="https://i.imgur.com/8TcOm6o.jpeg" width="200" alt="Logo"></a></p>

***

# CoachHub

CoachHub es una aplicación web la cual trata de hacerle la vida más facil a los entrenadores que desean llevar el análisis de datos al siguiente nivel y optimizar el rendimiento de sus equipos. Quiero que la aplicación permita a un entrenador facilitarle varias acciones como ver los partidos que vienen, guardarse las instrucciones tácticas, programar entrenamientos y observar estadísticas.

## Características principales:

- Recopilación de datos eficaz y sencilla.
- Creación de ejercicios (pizarra digital).
- Calendario con partidos y entrenamientos.

## Tecnologías usadas (en principio)
<p align="left"> <img src="https://cdn.worldvectorlogo.com/logos/git-bash.svg" alt="Bash" width="40" height="40"/>  
<img src="https://cdn.worldvectorlogo.com/logos/android-4.svg" alt="Android Studio" width="40" height="40"/> 
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="MySQL" width="40" height="40"/>
<img src="https://camo.githubusercontent.com/4965c61569069e46775836d78ee63f6cc0d8bac40bb2a0e638fe682e5aa18a95/68747470733a2f2f63646e2e776f726c64766563746f726c6f676f2e636f6d2f6c6f676f732f6769746875622d69636f6e2d322e737667" alt="GitHub" width="40" height="40"/>
</p>

## Base de datos (en principio)

```mermaid
erDiagram
    entrenamientos {
        int id
        text Ejercicios
        int fecha_id
        timestamp created_at
        timestamp updated_at
    }
    equipos {
        int id
        string Nombre
        string Categoria
        int  user_id
        timestamp created_at
        timestamp updated_at
    }
    fechas {
        int id
        int Tipo
        Date Dia
        string Inicio
        string Final
        int equipo_id
        timestamp created_at
        timestamp updated_at
    }
    jugadores{
        int id
        string Nombre
        int Dorsal
        string Posicion
        string Notas
        int Minutos
        int Amarillas
        int Rojas
        int Goles
        int Asistencias
        int equipo_id
        timestamp created_at
        timestamp updated_at
    }
    partidos{
        int id
        string Rival
        int fecha_id
        timestamp created_at
        timestamp updated_at
    }
    users{
        int id
        string name
        string email
        text password
        timestamp created_at
        timestamp updated_at
    }
    fechas ||--o{ entrenamientos : "id"
    users ||--o{ equipos : "id"
    equipos ||--o{ fechas : "id"
    equipos ||--o{ jugadores : "id"
    fechas ||--o{ partidos : "id"
```

## Estado del proyecto 📝

Por comenzar ⌛

## Contacto 💬 

Si surge algún problema con la aplicación, me lo puedes comunicar en docejavii@gmail.com.

## Autor

<a href="https://github.com/javiidoce"> Javier Melendo </a>

## Licencia ⚡

Copyright 2025 Javier Melendo Soler 

Por la presente se concede permiso, libre de cargos, a cualquier persona que obtenga una copia de este software y de los archivos de documentación asociados a utilizar CoachHub sin restricción, incluyendo sin limitación los derechos a usar, copiar, modificar, fusionar, publicar, distribuir, sublicenciar, y/o vender copias de CoachHub, y a permitir a las personas a las que se les proporcione el programa a hacer lo mismo, sujeto a las siguientes condiciones:  El aviso de copyright anterior y este aviso de permiso se incluirán en todas las copias o partes sustanciales del Software.  

EL SOFTWARE SE PROPORCIONA "COMO ESTÁ", SIN GARANTÍA DE NINGÚN TIPO, EXPRESA O IMPLÍCITA, INCLUYENDO PERO NO LIMITADO A GARANTÍAS DE COMERCIALIZACIÓN, IDONEIDAD PARA UN PROPÓSITO PARTICULAR E INCUMPLIMIENTO. EN NINGÚN CASO LOS AUTORES O PROPIETARIOS DE LOS DERECHOS DE AUTOR SERÁN RESPONSABLES DE NINGUNA RECLAMACIÓN, DAÑOS U OTRAS RESPONSABILIDADES, YA SEA EN UNA ACCIÓN DE CONTRATO, AGRAVIO O CUALQUIER OTRO MOTIVO, DERIVADAS DE, FUERA DE O EN CONEXIÓN CON EL SOFTWARE O SU USO U OTRO TIPO DE ACCIONES EN EL SOFTWARE.

