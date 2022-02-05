# Bienvenidos a nuestra primera misión!

Hola, soy Cesar Camilo tripulante de esta misión en **LaunchX**. Para nuestro primer reto necesitamos crear un botón con el cual iniciaremos nuestro viaje, usando la librería **ipywidget** de python. 

Para ello haremos uso de la extensión  [Jupyter](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) con la cual realizaremos las pruebas previas a nuestra misión.


## Necesitamos un manual

Antes de comenzar con el viaje, es muy importante tener nuestro **Manual de la nave**  por lo que insertaremos en la parte superior de nuestro archivo en Jupyter un bloque de **Markdown** con lo siguiente.

<pre><code># Manual de la Nave</code></pre>


## Necesitamos librerías!!!

Para continuar con nuestro despeje necesitaremos importar una librería la cual nos va dar ciertos componentes para que nuestra nave pueda despegar.  Para importarla agregamos un bloque de código con la siguiente instrucción:

<pre><code>pip install ipywidgets
</code></pre>
Ejecutamos la linea para posteriormente reiniciar. 


## ¿Código en una nave?

Para finalizar con el ejercicio y que nuestra nave pueda despejar necesitamos código, puede que si nunca hemos programado o usado python, pueda ser un poco complejo entenderlo pero lo que haremos a continuación sera copiar y pegar el siguiente bloque e insertarlo en el Jupyter.

<pre><code>import ipywidgets as widgets

ignition = widgets.ToggleButton(
    value=False,
    description='Iniciar Launch',
    button_style='success',
    tooltip='Engage your Launch',
    icon='rocket'
)

output = widgets.Output()

display(ignition, output)

def on_value_change(change):
    with output:
        if change['new'] == True:
            print("Nave Iniciada!")
        else:   
            print("Nave Detenida")

ignition.observe(on_value_change, names='value')
</code></pre>

Lo que hace este bloque es código es importar la librería **ipywidgets** con la cual podemos hacer uso de widgets interactivos, en el caso de esta misión vamos a ocupar un botón con el que podemos **Iniciar nuestra nave** o **Detener nuestra nave** a voluntad propia. 

## ¿Qué sigue?

Bueno esto aun no es el final de nuestro viaje, ya que apenas es solo el comienzo, en otros ejercicios estaremos probando algunos comandos de nuestra nave, mientras tanto a celebrar un pequeño logro 👩🏼‍🚀 

# Nuestra nave funciona y esto es solo el comienzo 🚀
