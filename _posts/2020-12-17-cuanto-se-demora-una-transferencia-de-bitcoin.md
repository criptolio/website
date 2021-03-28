---
layout: post
title:  "¿Cuánto se demora una transferencia de bitcoin?"
author: jp
categories: [ básico ]
image: assets/images/bitcoin/tiempo-transaccion-bitcoin.jpg
featured: false
hidden: false
---

Asumiendo el mejor de los casos, a continuación puedes ver el estimado de acuerdo al número de confirmaciones requeridas:

- 1 Confirmación: ~10 minutos
- 3 Confirmaciones: ~30 minutos
- 6 Confirmaciones: ~1 hora

La red Bitcoin procesa las transacciones por lotes (conjunto de transacciones o bloques), estos lotes se generan en promedio cada 10 minutos y se agrupan, principalmente, de acuerdo al costo por transacción (fee) pagado, es decir, las transacciones que pagan más se procesan primero.

El procesamiento de una transacción implica la validación de los datos de la misma, que esté estructurada adecuadamente, que tanto origen y destino sean direcciones válidas, que las direcciones origen tengan la cantidad suficiente estipulada en la transacción y que sí haya sido enviada por el propietario de las direcciones origen.

De acuerdo a lo anterior y para determinar cuánto se demora una transacción bitcoin, lo más importante es la primera confirmación de la red (cuando la transacción es procesada por la red) y nos obliga replantear la pregunta a **¿Cuánto se demora la primera confirmación?** ya que las siguientes confirmaciones se darán, de acuerdo a lo mencionado, cada 10 minutos en promedio.

## ¿Cuánto se demora la primera confirmación?

Como ya te podrás imaginar, en el mejor de los casos, la primera confirmación se demora lo mismo que el tiempo que toma en procesarse el siguiente lote de transacciones dentro de la red, por lo cual, la primera confirmación dependerá de qué tan rápido se generen los lotes (fuera de tu control) y de lo que hayas pagado (costo o fee) por la transacción (tu lo controlas).

Si bien no se puede determinar un tiempo exacto en el que una transacción será confirmada, si podrias tener un estimado de tiempo usando lo siguiente:

- Antes de enviar la transacción: puedes usar [Bitcoinfees.net](https://bitcoinfees.net/) para determinar cuánto pagar por la transacción (fee) y estimar el tiempo de la primera confirmación.
![Costo transacción bitcoin]({{ '/assets/images/bitcoin/costo-transaccion-bitcoin.png' | absolute_url }})
Recuerda que estos valores son variables y se deben consultar antes de hacer cada transacción.
- Una vez enviada la transacción: puedes usar [Blockonomics.co](https://www.blockonomics.co/) buscando el comprobante (Tx hash), mostrará el tiempo estimado para la primera confirmación.
![Tiempo estimado transacción bitcoin]({{ '/assets/images/bitcoin/tiempo-estimado-transaccion-bitcoin.png' | absolute_url }})

Adicionalmente, debes tener en cuenta lo siguiente:

- Si bien el promedio de generación de un lote es 10 minutos esto no siempre se cumple. Podría ser menos de 1 minuto o hasta horas.
- El promedio de 10 minutos es un valor configurado en la red y se garantiza validandolo y ajustando la dificultad de procesamiento de un lote cada 2016 lotes (bloques) lo que es aproximadamente cada 2 semanas, es decir, si el promedio en estos 2016 es por debajo de 10 minutos se aumenta la dificultad y en el caso contrario se disminuye, así la red se autorregula para que siempre se generen, en promedio, cada 10 minutos.
- Recuerda que mientras se confirma tu transacción otras personas pueden enviar transacciones con costos por transacción (fees) más altos, por lo cual, puede que estas se procesen primero y la tuya no sea incluida en el siguiente lote generado.

Finalmente, recuerda que una vez la transacción es procesada por la red, es **imposible de deshacer**.
