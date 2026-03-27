```
██╗  ██╗███████╗██╗     ██╗      ██████╗ 
██║  ██║██╔════╝██║     ██║     ██╔═══██╗
███████║█████╗  ██║     ██║     ██║   ██║
██╔══██║██╔══╝  ██║     ██║     ██║   ██║
██║  ██║███████╗███████╗███████╗╚██████╔╝
╚═╝  ╚═╝╚══════╝╚══════╝╚══════╝ ╚═════╝ 
```

📦 Plantilla base Java (Maven)

Esto es una plantilla que uso para mis proyectos de Java, para no tener que estar configurando todo desde cero cada vez.

¿Qué tiene?

En el pom.xml ya vienen varias dependencias que suelo usar siempre:

Lombok
Log4j (con SLF4J) +
JUnit 5 + 
Mockito + 
"Mockito + JUnit"
MySQL + 
HikariCP (pool de conexiones)

También incluye el archivo log4j.xml dentro de src/main/resources.

💡 ¿Por qué hice esto?

Esta "idea" se me ocurrió por el hecho de estar usando la misma plantilla para todos mis proyectos de Java, porque tenía que copiar y pegar cada una de las dependencias en los pom, al igual que el archivo de log4j.xml.
Dentro de IntelliJ existe la forma de poder crear plantillas para nuestros proyectos, que al seleccionarlas te crea el proyecto con el pom ya configurado y los archivos como el log4j.xml creado:

Para crearlo...

1. Clona el repositorio:

git clone git@github.com:ErickVelasquezTECH/base-template.git

2. Ábrelo en IntelliJ (con Open):

3. Ve a: 

File → New Projects Setup → Save Project as Template

Esto creará una plantilla en tu ordenador.


4. Cuando vayas a crear un proyecto nuevo:
-> Le das a New Project
-> En la izquierda te aparecerá Templates
-> Seleccionas esta plantilla

Y listo, ya tendrás todo configurado sin hacer nada más 😄

Importante:
El proyecto se crea ya con Maven (no te deja elegirlo, pero no hace falta)
Puede que el JDK no se configure bien automáticamente.

⚙️ Configurar el JDK (si falla)
A veces el proyecto se crea sin JDK o con otra versión y te salta el típico mensaje de "Download JDK".
Si te pasa:
File → Project Structure
Y ahí seleccionas Java 21 en el SDK y aplicas.

```
██╗   ██╗███████╗██╗      █████╗ ███████╗ ██████╗ ██╗   ██╗███████╗███████╗
██║   ██║██╔════╝██║     ██╔══██╗██╔════╝██╔═══██╗██║   ██║██╔════╝╚══███╔╝
██║   ██║█████╗  ██║     ███████║███████╗██║   ██║██║   ██║█████╗    ███╔╝ 
╚██╗ ██╔╝██╔══╝  ██║     ██╔══██║╚════██║██║▄▄ ██║██║   ██║██╔══╝   ███╔╝  
 ╚████╔╝ ███████╗███████╗██║  ██║███████║╚██████╔╝╚██████╔╝███████╗███████╗
  ╚═══╝  ╚══════╝╚══════╝╚═╝  ╚═╝╚══════╝ ╚══▀▀═╝  ╚═════╝ ╚══════╝╚══════╝

████████╗███████╗ ██████╗██╗  ██╗
╚══██╔══╝██╔════╝██╔════╝██║  ██║
   ██║   █████╗  ██║     ███████║
   ██║   ██╔══╝  ██║     ██╔══██║
   ██║   ███████╗╚██████╗██║  ██║
   ╚═╝   ╚══════╝ ╚═════╝╚═╝  ╚═╝
```

📚 Extra:
Esta plantilla está basada en otro repo que tengo con dependencias sueltas:
https://github.com/ErickVelasquezTECH/dependencies-snippets
