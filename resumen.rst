=======
Resumen
=======



.. _resumen-como-usar:

Cómo se usa
===========

En su forma más básica, sólo son necesarias dos cosas para para que el sistema
empiece a hacer llamadas:

1. Una lista con los números telefónicos.

2. Un audio con el mensaje a transmitir.

Estos datos (junto con otros detalles) se configuran dentro de una *campaña*.
Una vez configurada la campaña, Fonobot llamará a cada número y reproducirá el
audio correspondiente.  Se pueden tener varias campañas activas al mismo
tiempo, cada una configurada de manera independiente.



.. _resumen-numeros:

Listas de números telefónicos
=============================

Hay dos opciones para especificar la lista de números a llamar: proveer su
propia lista de números o utilizar una de las bases de datos integradas en el
sistema.


Bases de datos integradas
-------------------------

Puede utilizar una de las guías telefónicas provistas por el sistema, con la
posibilidad de llamar solamente a los números de una zona determinada.  Por
ejemplo, puede especificar que se usen solamente los números cercanos a su
comercio (en un radio de algunas pocas cuadras), o puede filtrarlos para llamar
a toda una ciudad o provincia.

Adicionalmente se puede filtrar por categoría de número, ya sean números
particulares o comerciales de un rubro determinado.  Consulte la documentación
sobre los :ref:`filtros de guías telefónicas <numeros-gt>` para más
información.


Lista de números personalizada
------------------------------

Si tiene una serie de números a los que desea llamara (como una lista de
clientes, por ejemplo), puede subir la lista al servidor y utilizarla tantas
veces como desee.  Se admiten los formatos más populares, como XLS (Excel) y
CSV.  Consulte la documentación sobre las :ref:`listas de usuario
<numeros-list>` para más información.



.. _resumen-audio:

Mensajes de audio
=================

La campaña no funcionará a menos que tenga un audio para reproducir.  Una vez
que suba su archivo de audio al sistema, quedará disponible en su biblioteca
personal y podrá asignarlo a las campañas que guste las veces que desee.

No hay restricciones respecto al origen del audio: :ref:`puede hacerlo grabar
con nuestros locutores <locuciones>`, contratar a un locutor externo, o
grabarlo usted mismo (*incluso desde su propio teléfono celular*).  El único
requisito a tener en cuenta es que debe tener los derechos correspondientes
para utilizar cualquier producción que pudiera estar cubierta bajo derechos de
autor (copyright).

Los archivos de audio deben tener una duración máxima de hasta **45 segundos**.
Se aceptan los formatos más populares (MP3, WAV, OGG, 3GP, etc.).

Consulte la documentación sobre la :ref:`administración de locuciones de audio
<mod-audio>` para una guía paso a paso para subir sus locuciones.



.. _resumen-respuestas-oyente:

Respuestas del oyente
=====================

Opcionalmente se puede configurar la reacción del sistema ante la respuesta del
oyente que recibe la llamada.  Lo más común es que al finalizar el mensaje se
presente al usuario con dos opciones, por ejemplo:

1. Si el oyente presiona la tecla ``1`` del teléfono se repetirá el mensaje.

2. Si el oyente presiona la tecla ``2``, usted recibirá un e-mail con el número
   telefónico del interesado.  Esto es útil para (por ejemplo) cerrar una
   venta.

La reacción ante la respuesta del oyente se puede configurar con la función de
:ref:`configuración de la campaña <mod-campa-edit>`.  Por defecto no se utiliza
ninguna de las opciones, por lo tanto la llamada se termina en cuanto finaliza
la reproducción del mensaje.

Tenga en cuenta que **debe informar al oyente** a través del mensaje de audio.
Por ejemplo, puede grabar al final de su mensaje la locución "si desea repetir
el mensaje pulse uno, si desea que lo contacte un representante pulse dos".



.. _resumen-credito:

Crédito
=======

Al finalizar cada llamada, el sistema calculará el costo y lo descontará del
crédito de la cuenta del usuario.  Cuando el crédito llegue a cero no se podrán
realizar más llamadas.  Puede consultar el saldo de su crédito en cualquier
momento en la :ref:`pantalla inicial <mod-dashboard>` de la aplicación, y puede
cargar crédito en su cuenta a través de la :ref:`función de recarga de crédito
<mod-recarga>`.  Las llamadas no atendidas **no** generan cargo alguno, es
decir, su costo es cero.

El costo de la llamada dependerá de la cantidad de repeticiones del mensaje y
de la tarifa vigente para el destino de la misma.  Por ejemplo, si se trata de
una llamada a un teléfono fijo de Buenos Aires (Argentina) tendrá un costo,
pero si es una llamada a un teléfono móvil, o a un destino del interior (larga
distancia), o incluso a otros países, el costo será diferente.  Puede consultar
las tarifas vigentes con la :ref:`función de tarifas <mod-tarifas>` en el menú
principal.

El costo en el cuadro tarifario es por unidad, y representa una emisión de
mensaje.  Si el mensaje se repite varias veces el costo se calculará de acuerdo
a la cantidad de repeticiones.  Por ejemplo, si el oyente pide repetir el
mensaje una vez, el costo facturado será el equivalente a dos llamadas (una
unidad por la emisión inicial, y una unidad por la repetición).



.. _resumen-horarios:

Horarios de las llamadas
========================

Las llamadas se realizarán solamente en los días y horarios que se especifiquen
en la :ref:`configuración de la campaña <mod-campa-edit>`.  Puede especificar
días de la semana individuales y horarios diferentes para cada día.

Al crear una campaña nueva se configuran por defecto los días **de lunes a
viernes de 11 a 17 hs**.

