# Despliegue de la aplicación pokedex.

1. Creamos nuestro proyecto en Firebase.

    ![image](https://user-images.githubusercontent.com/96387909/199774060-9aef5bdf-f9ae-4515-be6b-ee7d39fdda93.png)
    ![image](https://user-images.githubusercontent.com/96387909/199774204-aa0c1025-beb8-4a1b-b2f5-34291e658da6.png)

2. Una vez creado el proyecto Firebase nos mostrara varias herramientas, nos dirigiremos al menú de la izquierda y en compilación seleccionaremos Hosting y damos en el botón que dice comenzar.
   
   ![image](https://user-images.githubusercontent.com/96387909/199774739-098a455d-05ee-4656-84a2-eca3e274bb72.png)
   ![image](https://user-images.githubusercontent.com/96387909/199774932-e77ce6c1-d0b9-4015-83ad-383c20a55965.png)

3. Nos mostrara un página donde enseña como configurar el Hosting.
    
    ![image](https://user-images.githubusercontent.com/96387909/199775977-af591e64-ab32-47a2-8e11-dd0793c9687e.png)
    ![image](https://user-images.githubusercontent.com/96387909/199776048-d92665d0-b424-49fa-9a48-c5f01addc9b6.png)
    ![image](https://user-images.githubusercontent.com/96387909/199776109-e17a7e0f-1cac-4e73-9838-4ee7d5028771.png)
    
4.  Para los siguientes pasos puedes usar lo consola de Windows(CMD) o una terminal de VScode y nos ubicamos en la carpera "pokedex-angular".
    - En nuestro caso: `cd "\Downloads\pokedex-angular"`
5. Antes de iniciar con la configuración del hosting, ejecutamos el comando: `npm run build` para que nos cree la carpeta __dist\pokedex-angular__ que nos ayudara con el despliegue.
6. Luego se instala la Firebase CLI con el comando: `$ npm install -g firebase-tools`.
7. Después que se haya instalado el Firebase CLI, iniciamos sesión con la cuenta de Firebase con el comando: `$ firebase login`.

    ![image](https://user-images.githubusercontent.com/96387909/199783916-97368468-dd14-4043-baa8-6913f7fdf8c7.png)
    
8. Ahora inicializamos el proyecto con el comando: `$ firebase init`.
    ![image](https://user-images.githubusercontent.com/96387909/199784684-2c3a568b-b044-49e5-948c-4ed56f9e77c4.png)
   - Una vez le indiquemos que estamos listos, seleccionaremos la herramienta que vamos a usar de Firebase en este caso hosting.
      ![image](https://user-images.githubusercontent.com/96387909/199787275-b4a7c797-1d88-4b60-8526-4a7983012efc.png)
    - Luego nos preguntara que si usaremos un proyecto existente o crearemos un nuevo proyecto, en nuestro caso seleccionamos un proyecto existente.
      ![image](https://user-images.githubusercontent.com/96387909/199790087-7eef542a-c1f9-4c76-a21f-667755d99dc4.png)
    - Seleccionamos el proyecto creado en el primer paso llamado __pokedex-d__.
      ![image](https://user-images.githubusercontent.com/96387909/199791333-f2c2642a-d012-4528-bb80-38e768c19853.png)
   - Después nos preguntara "What do you want to use as your public directory?" (¿Qué quieres usar como tu directorio público?), al lado escribimos el nombre de la carpeta que se creó cuando hicimos `npm run build` que fue __dist\pokedex-angular__.
    - La siguiente pregunta que nos hace es "Configure as a single-page app (rewrite all urls to /index.html)?" la marcamos con un __Yes__
    - En las dos ultimas preguntas "Set up automatic builds and deploys with GitHub?" y "File dist/_pokedex-angular/index.html already exists. Overwrite?" 
 le decimos que __No__.
      ![image](https://user-images.githubusercontent.com/96387909/199807242-4e7402a3-42b6-4bdb-85bd-11a6e5441bdd.png)
    - __¡Inicialización de Firebase completa!__
    
 9. Para finalizar con el despliegue ejecutamos el comando: `firebase deploy`
 
    ![image](https://user-images.githubusercontent.com/96387909/199808589-3d444fd1-91eb-4baa-8568-0220913b12c1.png)
    
10. Ya tendremos nuestra aplicación pokedex desplegada. https://pokedex-d.web.app/

    ![image](https://user-images.githubusercontent.com/96387909/199809141-433f2da3-6e48-445f-9894-6c5ac2741d0b.png)



 



