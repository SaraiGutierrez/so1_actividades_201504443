#### Virginia Sarai Gutierrez Depaz 201504443

<br>

# Kernel
un software especial que forma parte importante del sistema operativo de cualquier ordenador. Por lo general, cuenta con la característica de que el mismo se ejecuta en un modo privilegiado, también llamado y mejor conocido como modo núcleo. Dentro de sus principales funciones, está el hecho de que facilita cualquier programa principal y necesario en el hardware del ordenador y es el encargado de gestionar cada uno de ellos para que funcionen de forma correcta.
</p>

![](../img/1.jpg)

# Tipos de Kernel y  Diferencias
Los diferentes sistemas operativos y dispositivos finales tienen diferentes tipos de kernels. Según sus características

- Kernel Monolitico:
Todo está incluido en un mismo espacio lógico o programa en el que se entrelazan todas las funciones o subrutinas.
Es totalmente responsable de la gestión de la memoria y los procesos, la comunicación entre procesos y proporciona funciones de soporte de controladores y hardware. Los sistemas operativos que utilizan kernels monolíticos incluyen Linux, OS X y Windows.

![](../img/2.png)


- Microkernel:
e caracteriza por un kernel muy pequeño con solo las funciones primitivas y llamadas al sistema para servicios básicos de espacios de direcciones, comunicación entre procesos y planificación básica.
Es deliberadamente pequeño para que una falla no destruya todo el sistema operativo. Pero para que pueda realizar las mismas funciones que el kernel grande, se divide en varios módulos. Como ejemplo de una aplicación, solo el componente Mach de OS X, ya que ningún sistema operativo tiene un microkernel hasta el momento.

![](../img/3.png)

- Kernel Hibrido:
Microkernel modificado que incluye más funcionalidades y las inserta dentro del kernel.
 La combinación de un kernel monolítico y un microKernel se denomina kernel híbrido. En este caso, los kernels grandes se vuelven más compactos y escalables. Otras partes del núcleo se pueden cargar dinámicamente. Esto ya sucede hasta cierto punto en Linux y OS X.

![](../img/4.png)

- Kernel Jerárquicos, Multicapas o en anillos: 
Hay diferentes capas o anillos en función de los componentes del kernel y cada uno tiene un nivel jerárquico siendo los más externos los de menores privilegios.

![](../img/5.png)

- Kernel Distribuido:
Separa sus componentes en servidores que se distribuyen en uno o varios nodos y el reducido kernel se encarga simplemente de la comunicación de los componentes

![](../img/6.png)

- ExoKernel: no proveen abstracciones de hardware, pero permiten el uso de librerias que brindan mayor funcionalidad debido al acceso directo o casi directo al hardware.

![](../img/7.png)

<br>

# User vs Kernel mode

- Modo Usuario: 
cuando se inicia un programa en un sistema operativo, digamos Windows, se inicia el programa en modo de usuario. Y cuando un programa en modo usuario solicita ejecutarse, Windows crea un proceso y un espacio de direcciones virtuales (espacio de direcciones para ese proceso). Los programas de modo de usuario tienen menos privilegios que las aplicaciones de modo de usuario y no se les permite acceder a los recursos del sistema directamente. Por ejemplo, si una aplicación en modo de usuario desea acceder a los recursos del sistema, primero deberá pasar por el kernel del sistema operativo mediante llamadas al sistema.  

- Modo Kernel:
El kernel es el programa central en el que se basan todos los demás componentes del sistema operativo, se utiliza para acceder a los componentes de hardware y programar qué procesos deben ejecutarse en un sistema informático y cuándo, y también administra la interacción entre el software y el hardware de la aplicación. . Por lo tanto, es el programa más privilegiado, a diferencia de otros programas, puede interactuar directamente con el hardware. Cuando los programas que se ejecutan en modo de usuario necesitan acceso al hardware, por ejemplo, una cámara web, primero tiene que pasar por el núcleo mediante una llamada al sistema y, para llevar a cabo estas solicitudes, la CPU cambia del modo de usuario al modo de núcleo en el momento de la ejecución. Después de completar finalmente la ejecución del proceso, la CPU vuelve a cambiar al modo de usuario .

![](../img/8.png)