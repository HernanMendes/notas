# Notas
---
## *MongoDB*
Date: 2022-03-09

Gestor de bases de datos **No Relacionales**(NO-SQL). Orientada a *colecciones* y *documentos*, en vez de *tablas* y registros*. Dichos documentos tienen formato **JSON**.

[Documentación](https://docs.mongodb.com/)

---
## *ETL* - Extract, Transform, Load.
Date: 2022-03-09

Proceso de extraer, transformar t cargar data desde diferentes fuentes a un *data warehouse* u otros repositorios de código unificado de data. Integreción de datos.
  
[Fuente](https://www.ibm.com/cloud/learn/etl)

---
## *ELT* - Extract, Load, Transform.
Date: 2022-03-09

Cargar la data cruda oara luego ser transformada.
  
[Fuente](https://www.ibm.com/cloud/learn/etl)

---
## *Pre-Scrapping*
Date: 2022-03-09

¿Qué secciones y URL voy a explorar? **Crawler**

---
## *Docker*
Date: 2022-03-09

Herramienta para crear, desplegar y correr apps usando **contenedores**.
Los contenedores permiten desplegar una aplicación con todas las librerías, paquetes o dependencias que necesite.
Así nos aseguramos que la app correrá en cualquier máquina independientemente de la configuración del sistema.

A diferencia de una máquina virtual, Docker, en vez de creat dodo un nuevo sistema de archivos con una imágen completa del *SO*, permite que las aplicaciones usen el mismo kernel de Linux que el sistema y sólo se le agreguen aquellas dependencias que no se encuentran en el sistema de destino. Esto implica una mejor performance, reduce el tamaño de la aplicación, independecia, abstracción, automatización y aislar procesos.

![docker_vs_vm](https://s3.amazonaws.com/oodles-technologies1/blog-images/af7d2186-b715-4f67-992a-c34a2c180eb7.jpeg)


[Docker para todes](https://docs.google.com/presentation/d/1MZ2QnAZ99AbhCXh8hvAzGdG9YJQaZT5R2WwhITITw48/edit?usp=sharing)

[Docker_introduccion](https://drive.google.com/file/d/17P98VrLISI3zWPmpYBsAySNYzBHL1u9q/view?usp=sharing)

[Instalacion](https://phoenixnap.com/kb/install-docker-on-ubuntu-20-04)

---
## _Torrent_
Date: 2022-03-11

Es un archivo enviado a través del protocolo **BitTorrent**. Son diferentes a las descargas regulares ya que son descargados desde varios servidores al mismo tiempo.

[Fuente](https://techterms.com/definition/torrent)

---
## _BitTorrent Protocol_
Date: 2022-03-11

Usa múltiples computadoras para transferir un único archivo, en consecuencia reduce el ancho de banda requerido por cada servidor. Cuando una descarga *torrent* inica, el sistema BT localiza difetentes computadoras con el archivo completo y descarga diferentes partes del archivo desde cada computadora. Esto conlleva menor BW y mayor velocidad

[Fuente](https://techterms.com/definition/bittorrent)

---
## _Seeders_
Date: 2022-03-11

Usuarios que tienen el archivo completo y lo están compartiendo. Son quienes suben la data.

A mayor cantidad de seeders, mayor velocidad de descarga.

[Fuente](https://es.ccm.net/faq/3149-que-son-los-seeders-y-leechers)

---
## _Leechers_
Date: 2022-03-11

Los usuarios que están bajando la data.

[Fuente](https://es.ccm.net/faq/3149-que-son-los-seeders-y-leechers)

---
## _YAML_
Date: 2022-03-11

Lenguaje de serialización de datos a menudo usado para escribir archivos de configuración.

[yaml](https://yaml.org/)
[Fuente](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)


---
## _Install/Uninstall .deb files_

Date: 2022- 03-14

1. To install a .deb file, simply Right click on the .deb file, and choose Kubuntu Package Menu->Install Package.

2. Alternatively, you can also install a .deb file by opening a terminal and typing:
    ```sh
    sudo dpkg -i package_file.deb
    ```
3. To uninstall a .deb file, remove it using Adept, or type:
    ```sh
    sudo apt-get remove package_name
    ```
[Fuente](https://help.ubuntu.com/kubuntu/desktopguide/C/manual-install.html)

---

## _How to install tar.gz in ubuntu 20.04_
Date: 2022-03-14
```sh
tar -xzf archive-name.tar.gz
cd archive-name
./configure
make
sudo make install
```
  
[Fuente](https://www.codegrepper.com/code-examples/shell/how+to+install+tar.gz+in+ubuntu+20.04)

---
## _Anaconda_
Date: 2022-03-14

Verificar que esté instalado y la versión
```sh
conda --version
```
Listar entornos
```sh
conda env list
```
Eliminar entorno
```sh
conda-env remove -n nombre_entorno
```
Crear entorno
```sh
conda create -n nombre_entorno python=3.10
```
Activar entorno
```sh
conda activate nombre_entorno
```

Luego instalas los paquetes que desees. EJ:
```sh
pip install requests
```
Listar paquetes instalados en el entorno
```sh
pip freeze
```

```sh
mkdir intro_scrapping
cd intro_scrapping
mkdir requirements
pip freeze > requirements/production.txt
```
---
## _Docker_
Date: 2022-03-14

INSTALAR PORTAINER

[DockerHub](https://hub.docker.com/)


Descargar Imagen de Mongo
```sh
(sudo) docker pull mongo
```
Correr Imagen
```sh
docker run -p 37017:27017 --name mi_mongo -d mongo:latest
```
Listar Cointariners Activos
```sh
docker ps
```
Frenar container
```sh
docker nombre_cointainer
```
Eliminar
```sh
docker rm nombre_cointainer
```

---
## _requests.session()_
Date: 2022-03-16

El objeto *Session* nos permite persistir ciertos parametros a través de las *requests*. También persiste las *cookies* a traves de todas las requests hechas desde la  misma instancia Session. Esto resulta en una significante mejora de la performance ya que la misma coneccion TCP será retilizada para las distintas requests hechas desde el mismo host.

[Documentación](https://docs.python.org/3/library/concurrent.futures.html#module-concurrent.futures)

---
## _query_
Date: 2022-03-16

Una *query* es una consulta por data o informacion a una base de datos la cual devolverá una respuesta según lo consultado.

SQL = Structured **Query** Language

![query](https://media.istockphoto.com/vectors/database-query-vector-id1299408835?k=20&m=1299408835&s=170667a&w=0&h=kKhGqYgYycFtDoJ51D0egBsOrgPIkDkSm-gfrgCCgnI=)
[Fuente](https://www.techopedia.com/definition/5736/query)

---
## _future.result()_
Date: 2022-03-17

Retorna el valor retornado por la función ejecutada por el *executor*.
  
[Documentación](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.Future.result)

---
## _locals() - Python function_
Date: 2022-03-17

Retorna un diccionario que contiene las variables definidas en el scope local donde fueron llevadas.

[Fuente](https://appdividend.com/2019/08/01/python-locals-example-locals-function-tutorial/)  
[Documentación](https://docs.python.org/3/library/functions.html#locals)

---
## _argparse_
Date: 2022-03-17

El modulo *argparse* hace más fácil escribir interfaces a través de lineas de comandos amigables para el usuario. Define que argumentos son requeridos, genera mensajes de ayuda y error. 
  
[Documentación](https://docs.python.org/3/library/argparse.html)

---
## _API - Application Programming Interface_
Date: 2022-03-18

Es un software intermediario que permite que dos aplicaciones interactuen entre ellas.

![que_es_api](https://i.pinimg.com/originals/17/fc/eb/17fcebe8a0efd8472132d184a1c79cb1.png)
![api_interface](https://www.astera.com/wp-content/uploads/2020/01/rest.png)
![api_interface2](https://www.altexsoft.com/media/2019/06/Screenshot_1.png)

[Fuente1](https://www.mulesoft.com/resources/api/what-is-an-api)

---
## _ORM_
Date: 2022-03-18

Object-Relational mapping, o lo que es lo mismo, mapeo de objeto-relacional, es un modelo de programación que consiste en la transformación de las tablas de una base de datos, en una serie de entidades que simplifiquen las tareas básicas de acceso a los datos para el programador.
  
[Fuente](http://www.tuprogramacion.com/glosario/que-es-un-orm/)

---
## _Payload_
Date: 2022-03-18

Cuando la data es enviada a través de Internet, cada unidad transmitida incluye el *header* y la *data* propiamente dicha. El *header* identifica la fuente y el destino de los paquetes, mientras que la data propiamente dicha se denomina **payload**. La informacipon del header sólo es usada en el proceso de transmisión, es separada del paquete cuando llega a su destino. El **payload** es la única que recibe el sistema de destino.

[Fuente](https://techterms.com/definition/payload)

---
## _Concurrency and Parallelism_
Date: 2022-03-18

**Concurrency:** 
Concurrency relates to an application that is processing more than one task at the same time. Concurrency is an approach that is used for decreasing the response time of the system by using the single processing unit. Concurrency is creates the illusion of parallelism, however actually the chunks of a task aren’t parallelly processed, but inside the application, there are more than one task is being processed at a time. It doesn’t fully end one task before it begins ensuing. 
Concurrency is achieved through the interleaving operation of processes on the central processing unit(CPU) or in other words by the context switching. that’s rationale it’s like parallel processing. It increases the amount of work finished at a time.

**Parallelism:** 
Parallelism is related to an application where  tasks are divided into smaller sub-tasks that are processed seemingly simultaneously or parallel. It is used to increase the throughput and computational speed of the system by using multiple processors. It enables single sequential CPUs to do lot of things “seemingly” simultaneously. 

Parallelism leads to overlapping of central processing units and input-output tasks in one process with the central processing unit and input-output tasks of another process. Whereas in concurrency the speed is increased by overlapping the input-output activities of one process with CPU process of another process. 
  
[Fuente](https://www.geeksforgeeks.org/difference-between-concurrency-and-parallelism/#:~:text=Concurrency%20is%20the%20task%20of,of%20running%20multiple%20computations%20simultaneously)

---
## _XPath_
Date: 2022-03-21

XPath stands for XML Path Language. It uses a non-XML syntax to provide a flexible way of addressing (pointing to) different parts of an XML document. It can also be used to test addressed nodes within a document to determine whether they match a pattern or not.

![xpath](https://www.scientecheasy.com/wp-content/uploads/2019/08/xpath-syntax.png)

[Fuente](https://developer.mozilla.org/en-US/docs/Web/XPath)  
[XPath CheatSheet](https://devhints.io/xpath#class-check)
[XPath Tutorial](https://www.w3schools.com/xml/xpath_intro.asp)

---
## _Twitter API Elevated Access Level Questions_
Date: 2022-04-01

- In English, please describe how you plan to use Twitter data and/or APIs. The more detailed the response, the easier it is to review and approve.
- Are you planning to analyze Twitter data? Please describe how you will analyze Twitter data including any analysis of Tweets or Twitter users.
- Will your App use Tweet, Retweet, Like, Follow, or Direct Message functionality? Please describe your planned use of these features.
- Do you plan to display Tweets or aggregate data about Twitter content outside Twitter? Please describe how and where Tweets and/or data about Twitter content will be displayed outside of Twitter.
- Will your product, service, or analysis make Twitter content or derived information available to a government entity? Please list all government entities you intend to provide Twitter content or derived information to under this use case.

## _pandas.DataFrame.explode_
Date: 2022-04-07

Transforma todos los elementos de una lista (or *list-like*) en una fila y replica los índices.

```python
df['SplitTitle'] = df['Title'].apply(lambda x : x.split(' '))

df = df.explode('SplitTitle')

df.loc[1]
```

[Documentation](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.explode.html)

---

## _Regular Expressions (RegEx)_
Date: 2022-04-08

Define a search pattern that can be used to search for things in a string.
  
[freeCodeCamp Video](https://www.youtube.com/watch?v=ZfQFUJhPqMM)


---
## _Natural Language Processing (NLP)_
Date: 2022-04-08

Se refiere a la rama de la IA que se ocupa de darle a las computadoras la habilidad de entender texto y palabras escritas de la misma manera que lo pueden hacer los seres humanos.
  
[Fuente - IB;](https://www.ibm.com/cloud/learn/natural-language-processing)

---
## _Error Handling - Python_
Date: 2022-04-20

```python
try:
    f = open('test_file.txt') #this file exist
    
    if f.name == 'currupt_file.txt':
        raise Exception     # Raise our own exceptions
    
    var = bad_var   #NameError exception
except FileNotFoundError:   #catch this first if file not exist
    print('Sorry! This file does not exist')
except Exception as e:  # catch any exception
    print('Sorry! Something went wrong') #custom mensagge
    print(e) # print error message
else:
    # Executed if the 'try' clause does not raise an execption
    print(f.read())
    f.close()
finally:
    # Executed no matter what happens
    print("Executing Finally...")
    pass
```
  
[Video Example](https://www.youtube.com/watch?v=NIWwJbo-9_8)

---
## _Bounding Boxes_
Date: 2022-04-25

Conventions used in specifying a bounding box:

There are 2 main conventions followed when representing bounding boxes:

1. Specifying the box with respect to the coordinates of its top left, and the bottom right point.<br>
![bbox_1](.images/bbox_1.jpeg)
2. Specifying the box with respect to its center, and its width and height.<br>
![bbox_2](.images/bbox_2.jpeg)

**Converting between the conventions:**

We can convert between the different forms of representing the bounding box, depending on our use case.

1. xc = ( x1 + x2 ) / 2
2. yc = ( y1 + y2 ) / 2
3. width = ( x2 — x1)
4. height = (y2 — y1)
  
[Fuente](https://medium.com/analytics-vidhya/basics-of-bounding-boxes-94e583b5e16c)

---
## _Selenium Ubuntu Setup_
Date: 2022-05-02

1. [Install Google Chrome](https://itsfoss.com/install-chrome-ubuntu/)
   
    ```sh
    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
    ```
    ```sh
    sudo dpkg -i google-chrome-stable_current_amd64.deb
    ```
    ```sh
    google-chrome --version
    ```
    ```sh
    wherei google-chrome
    ```
2. Install Chrome Driver
    [Download](https://chromedriver.chromium.org/). Tiene que coincidir la versión de chrome con la del driver.<br>
    ```sh
    unzip chromedriver_linux64.zip
    ```
    ```sh
    chmod +x chromedriver
    ```
    Mover a carpeta compartida
    ```sh
    sudo mv ~/chromedriver /usr/local/share/chromedriver
    ```
    Create links
    ```sh
    sudo ln -s /usr/local/share/chromedriver /usr/local/bin/chromedriver
    sudo ln -s /usr/local/share/chromedriver /usr/bin/chromedriver
    ```
    Check chrome driver version
    ```sh
    chromedriver --version
    ```
3. Install Selenium
   ```sh
    pip install selenium
    ```
[Markdown CheatSheet](https://www.markdownguide.org/cheat-sheet/)

---
## _Cron/Crontab_
Date: 2022-05-09

Administrador de linux que nos permite controlar los procesos que se ejecutan en segundo plano en intervalos de tiempo.

Manual
```sh
man crontab
```
List process
```sh
crontab -l
```
Remove process
```sh
crontab -r
```
Edit
```sh
crontab -e
```

**Example 1**
Imprimir la hora a cada minuto en un archivo de texto
```sh
 * * * * * date >> /home/hernan/Desktop/hora.txt
```
**Example 2**
Execute python script the first day of every month at 00:01:00
```sh
1 0 1 * * /home/hernan/anaconda3/envs/bbhits/bin/python /home/hernan/Desktop/BB_Vision/Twitter_bots/load_bots_to_db/main.py
```

**Salir de NANO**
CTRL + O
ENTER
CTRL + X


[Video](https://www.youtube.com/watch?v=lvW6Fw3Ghy8)
[Crontab Guru](https://crontab.guru/)
---
## _Cantidad de Request - Twitter API_
Date: 2022-04-26

Hashtag Count - Top 5000 TMDB
| Probe # | Set           | API Version |   EndPoint          | Total Count | Time     | Date |
| -----   | -----         | -----       | -----               | -----       | -----    | -----|
| 1       | top 5000 tmdb | v2          | Recent Tweets Count | 1638414     | 233min   | 27 abr 2022 16∶24∶35 |
| 2       | top 5000 tmdb | v2          | Recent Tweets Count | 1670701     | 255min   | 28 abr 2022 09∶34∶38 |
| 3       | top 100  imdb | v2          | Recent Tweets Count | 212522      | 0min 30s | 28 abr 2022 09∶53∶07 |
| 4       | top 100  imdb | v2          | Recent Tweets Count | 355676      | 0min 31s | 28 abr 2022 10∶26∶49 |
| 5       | top 100  imdb | v2          | Recent Tweets Count | 415416      | 0min 29s | 28 abr 2022 15∶06∶35 |
| 6       | imdb/tmdb clean| v2          | Recent Tweets Count | 1764389     | 244min   | 28 abr 2022 15∶06∶35|
| 7       | 5000 tmdb mov | v2          | Recent Tweets Count | 4324384     | 241min   | 02 may 2022 17∶10∶25 |
| 8       | 5000 tmdb tv | v2          | Recent Tweets Count | 5662733     | 247min   | 03 may 2022 10∶14∶58 |

9774 488min
date/date set

**Get Gender or Age**<br>
Twitter API no provee información de edad o género.<br>
Se podría determinar usando alguna AI analizando las imagenes de perfil y/o nombres de usuario.

- [X] Hashtag Count
- [X] genero
- [X] con v2 buscar query hashtag de cada tweet y ver location
- [X] PROBAR SI CON PAGINATOR ME TRAE USERS,PLACE => SI
- [X] probar busqueda context.entity => una vez que tenemos todos los tweets filtramos por user.location, context.entity
- [X] CONTEXT, para diferenciar de un libro, juego, etc. Twitter lo diferencia? => filtrar por context, magia NO. En v1 no lo tenemos, pero podemos obtener el ID y buscar en v2
- [ ] comparar esto con busqueda hashtag + place_country v1
- [X] que api/version/access_level usamos? => se podrían crear varias cuentas de v2 / Elevated Access, v1 va en desuso
- [X] Volver a hacer el count con una lista actualizada de tmdb!! => 4324384(movies) y 5662733(tv)
- [X] cuantas request/min puedo hacer con paginator/recent_search? => 450 requests/15min, hasta 100tw/requests
- [X] probar multicuenta con diferentes workers => BIEN
- [X] tomar todos los tweets de un set
- [X] Guardar datos de los bots en un db
- [ ] Rotar keys
- [ ] Me bloquea la IP?
- [ ] Filtrar por domain/entity
- [ ] Clasificar según pais
- [ ] Como se guardan las keys?
- [ ] Como generar cuentas para bots?
- [ ] Reset keys cada mes (crontab)
- [ ] automatic detect monthly cap usage. client. error. respone.content
- [ ] concurrent
- [ ] crear al menos 15 cuentas
- [ ] crear script que se fije en que fecha se bloqueo la cuenta y si paso un mes la desbloquee
---
## _Title_
Date: 2022-03-14

```sh
codigo
```
  
[Markdown CheatSheet](https://www.markdownguide.org/cheat-sheet/)

---
## _DUDAS A DESARROLLAR_

pruebas unitarias? <br>
milestone?<br>
AirFlow?<br>
Azzure?<br>
AWS?<br>
VPN?<br>
Pipeline?<br>
PEP8?<br>
global python<br>
html.unescape python<br>
concurrent vs multiprocesing (libraries)<br>
multiprocesing vs multithreading<br>
digitalocean<br>
proxy<br>
expressvpn (linux)<br>
wave <br>
crear indice para las notas <br>
curl (api)<br>
cloudflare
---

