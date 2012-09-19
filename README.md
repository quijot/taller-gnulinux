# Encuentro 4

## De paquetes, gestores y repositores

Todo lo que queramos hacer en GNU/Linux tiene una gran (des)ventaja: hay entre álef<sub>0</sub> y álef<sub>1</sub> opciones (álef=&#1488;), es decir: hay libertad, lo que nos obliga a informarnos, a estudiar las opciones para saber cuál se ajusta mejor a nuestra necesidad.

El __instalar programas__ no es la excepción. En GNU/Linux tenemos varios caminos. Sin embargo, se podría decir que lo más recomendable es utilizar el __gestor de paquetes__ e instalar los __paquetes de software__ de los __repositorios__ oficiales de nuestra distribución... ¡'perá 'perá! ¡No te vayas!

Cebate un mate y veamos...

### ¿Qué es un repositorio?

Es un lugar donde se almacenan programas o __paquetes de software__. Se puede decir que es una base de datos de programas. Entonces, cada distro mantiene oficialmente un conjunto de repositorios que constituyen una gran base de datos centralizada con todo el software de su distribución de GNU/Linux.

Ejemplo: el [main repo](http://ppa.launchpad.net/fta/ubuntu/dists/quantal/main/) de Ubuntu quantal...

### ¿Qué es un paquete?

Un _paquete de software_ es una serie de programas que se distribuyen conjuntamente, porque el funcionamiento de cada uno complementa a los otros o requiere de los otros o porque son afines o porque....

Ejemplo: LibreOffice es un paquete con varios programas.

### ¿Qué es un gestor de paquetes?

Para permitir a los usuarios con permiso instalar, desinstalar o actualizar _paquetes_ desde los _repositorios_, la mayoría de las distribuciones de GNU/Linux traen su _gestor de paquetes_.

A su vez, se encargan de:

- controlar que los paquetes estén bien instalados;
- __ofrecer actualizaciones__ cuando las mismas aparecen en los repositorios y
- __mantienen las dependencias__ entre paquetes: si un paquete se recuesta en otro, el sistema se encarga de instalar éste primero.

También podemos, a riesgo propio, agregar repositorios para que el gestor tenga en cuenta los paquetes allí ofrecidos.

De otra manera, deberíamos hacer este trabajo a mano, lo cual puede resultar engorroso.

## Instalemos

> Como todos los programas en GNU/Linux, los gestores de paquetes también se pueden manejar por consola.

Ahora instalemos desde consola programas copados para la consola.

    # Debian, Ubuntu (con sudo)
    $ apt-get install tree, mp3blaster, ranger, lynx

    # Mandriva, Mageia
    $ urpmi tree, mp3blaster, ranger, lynx

    # RedHat, Fedora
    $ yum install tree, mp3blaster, ranger, lynx

    # SuSE
    $ yast?

etc...

## ToDo

- instalar un programa que no está en el repo
    - está el paquete en otro lado
    - no está el paquete -> compilar
- qué es autopackage?
- hablar de quién y cómo hacen/mantienen los paquetes