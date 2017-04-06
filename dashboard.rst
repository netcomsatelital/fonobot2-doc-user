.. _mod-dashboard:

=========
Dashboard
=========

La pantalla de resumen o *dashboard* muestra una vista general del estado de la
cuenta.  Se muestra la siguiente información:

- Botón :guilabel:`Cargar saldo`.  Permite cargar saldo en la cuenta a través
  de los medios de pago habilitados (*Mercadopago* y *Paypal*).

- Crédito restante en la cuenta.  Este valor va decreciendo a medida que se
  realizan las llamadas.

- Qué campañas están funcionando en ese momento.

- Cuáles son las campañas que tienen menor cantidad de números.  Cuando una
  campaña se queda sin números para llamar finaliza automáticamente.


- Estadísticas por día de la semana.  Por cada día se grafica la cantidad
  relativa de llamadas:

      .. image:: _static/screen-mod-dashboard-01.png
        :align: center
    
    - La barra de color verde representa la cantidad de llamadas *entregadas*,
      es decir aquellas llamadas que fueron atendidas y escuchadas
      completamente al menos una vez.

    - La barra de color celeste representa la cantidad de llamadas *atendidas*,
      es decir las llamadas en las que el oyente contestó el teléfono.

    - La barra de color naranja representa la cantidad total de llamadas
      *enviadas* a la red telefónica, pero que no pudieron concretarse por
      alguna razón ajena al sistema.  Suele ocurrir con números inválidos,
      dados de baja, o simplemente por problemas temporales de la red
      telefónica (por ejemplo, un cliente de telefonía celular con problemas en
      la celda donde está conectado, problemas en el cableado o la central
      telefónica del cliente, etc.).

- Estadísticas por hora.  Análogo a las estadísticas por día de la semana, pero
  mostrando un resumen de las mejores horas para llamar.  Combinando esta
  información con la de la estadística anterior se puede tener una idea de qué
  días y horarios son los mejores para obtener la mejor respuesta de una
  campaña en particular.

  .. image:: _static/screen-mod-dashboard-02.png
    :align: center
