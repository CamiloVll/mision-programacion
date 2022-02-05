# ¿Nueva misión?

Así es, una nueva misión esta en proceso, para lo cual tendremos que mostrar los niveles de oxigeno que tenemos, ademas de calcular la en tiempo que tardaríamos en alcanzar la velocidad que queremos para nuestra nave. 


### Primeros pasos

Nuestra primer parada sera para definir con los bloques de **Markdown** el siguiente bloque.

<pre><code>## Niveles de Oxígeno
Muestra diez minutos de niveles de oxígeno en tu nave.
</code></pre>

### Librerías

Para conocer el oxigeno de nuestra nave utilizaremos 2 librerías **matplotlib**, **numpy** cuya función es hacer gráficos a partir de datos contenidos en listas o arrays. Nos es de vital importancia instalar las librerías para que podamos continuar.

<pre><code> pip install matplotlib
 pip install numpy
</code></pre>

### Código

Finalizando con el reto, lo que basta es copiar el siguiente bloque y ver la magia que ocurre

<pre><code> 
import numpy as np
import matplotlib.pyplot as plt
data = np.random.default_rng(12345)
oxy_nums  =  data.integers(low=0,  high=10,  size=10)

plt.bar(range(len(oxy_nums)),  oxy_nums)
plt.show()
</code></pre>

## Cálculos de nuestra nave

Es importante conocer nuestra nave, para ello haremos la prueba de su velocidad.
Como siempre antes de continuar nombramos **Markdown** para conocer los detalles de las acciones que hacemos en la nave.

<pre><code>## Velocidad de la nave
Muestra los segundos necesarios para pasar de 0 a determinados metros por segundo, dada la aceleración de la nave en metros por segundo.
</code></pre>
 
 ### Código
 
 Al querer averiguar el tiempo para alcanzar la velocidad deseada necesitamos hacer lo siguiente: 
 
 <pre><code>
 endVelocity  =  39937
 startVelocity  =  0
 acceleration  =  9.8 

time  =  (endVelocity  -  startVelocity)  /  acceleration
print("Tiempo para alcanzar la velocidad deseada = ",  time)
</code></pre>
 
 Podemos jugar con lo valores y obtener distintos resultados, ya dependerá de que tanto queremos tunear nuestra nave!

