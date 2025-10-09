🖥️ Configuración DHCP en un router

El bloque que tenemos es:

ip dhcp pool CASA
 network 192.168.1.0 255.255.255.0
 default-router 192.168.1.1
 dns-server 192.168.1.1
 lease 7

📌 Explicación línea a línea
🔹 ip dhcp pool CASA

Crea un “pool” de direcciones DHCP.

Un pool es como una bolsa de direcciones IP que el router va a repartir a los dispositivos de la red.

El nombre "CASA" es solo una etiqueta para identificar ese conjunto de configuraciones.

👉 Piensa en un guardia en la entrada de un parking: “este es el parking CASA, y aquí están las plazas que voy a dar a los coches”.

🔹 network 192.168.1.0 255.255.255.0

Define qué red usará el router para dar direcciones.

Aquí se usa la red 192.168.1.0 con máscara 255.255.255.0.

Esa máscara significa que estamos usando un bloque de tipo /24 (24 bits para la red, 8 para los hosts).

¿Qué implica?

Dentro de este bloque hay 256 direcciones en total.

2 se reservan (la primera para identificar la red y la última para broadcast).

Quedan 254 direcciones disponibles, que van de la 192.168.1.1 a la 192.168.1.254.

👉 En nuestro parking, esto equivale a decir: “el parking CASA tiene plazas numeradas de la 1 a la 254”.

🔹 default-router 192.168.1.1

Es la puerta de enlace o gateway.

Significa que todos los dispositivos que reciban una IP también sabrán que deben enviar su tráfico al 192.168.1.1 para salir a Internet.

Normalmente esta dirección corresponde al propio router.

👉 En el parking, sería como la salida principal que todos usan para salir a la carretera.

🔹 dns-server 192.168.1.1

Indica qué servidor DNS (el que traduce nombres como google.com en direcciones IP) van a usar los clientes.

En este caso, se está configurando para que sea el propio router (192.168.1.1).

El router a su vez preguntará a otros servidores DNS en Internet (como Google 8.8.8.8 o Cloudflare 1.1.1.1).

👉 En el parking, esto sería como el “guía” que te traduce las direcciones: “quiero ir a la calle Google” → el DNS te dice qué número de casa es.

🔹 lease 7

Es el tiempo de préstamo de la dirección IP.

Aquí, cada dispositivo que reciba una IP la podrá usar durante 7 días.

Cuando se acaba el tiempo, el dispositivo pide al router renovar la dirección.

👉 En el parking: cada coche alquila una plaza durante 7 días, y si sigue aparcado debe renovar el alquiler.

📝 Resumen simple

Pool CASA → nombre del conjunto de direcciones.

Red 192.168.1.0/24 → el rango disponible para repartir.

Gateway 192.168.1.1 → salida hacia Internet.

DNS 192.168.1.1 → traductor de nombres en números IP.

Lease 7 → el tiempo que dura la IP prestada (7 días).

🚀 Ejemplo práctico

Con esta configuración, si enciendes 3 dispositivos en casa:

Laptop recibe 192.168.1.2

Smartphone recibe 192.168.1.3

Consola recibe 192.168.1.4

Todos saben que deben usar el 192.168.1.1 como puerta de enlace y servidor DNS.