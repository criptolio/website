---
layout: post
title:  "¿Cómo hacer un depósito o transferencia en Bitcoin?"
author: jp
categories: [ básico ]
image: assets/images/bitcoin/deposito-transferencia-bitcoin.jpg
featured: false
hidden: false
---

Una vez tengas tu [wallet configurada]({% post_url 2020-12-14-que-es-un-wallet-bitcoin %}) podrás realizar depósitos o transferencias dentro de la red Bitcoin.

En ambos casos debes tener en cuenta lo siguiente:
- Una dirección bitcoin es el equivalente al número de cuenta de una entidad bancaria.
- Hasta el momento existen tres diferentes tipos de direcciones bitcoin y aunque tienen nombres técnicos acá solo mencionaremos que pueden empezar por 1, por 3 o por bc1.
- Para realizar una transacción, depósito o transferencia, debes saber la dirección, cantidad y el costo (fee) que se va a pagar por dicha transacción.
- Una vez una transacción se haya enviado a la red **no se puede deshacer**, sin embargo, se deberá esperar la confirmación de la red para considerarla como completada.
- El tiempo de confirmación (en el que la procesa la red) de una transacción dependerá del costo (fee) que se haya pagado por la misma y de la congestión de la red.

## Depositos

En la wallet busca el menú **Depositar** o **Recibir**, aparecerá una dirección similar a alguna de las siguientes:

-   Si empieza por 1: 1DSh7vX6ed2cgTeKPwufV5i4hSi4pp373h
-   Si empieza por 3: 3KqyQBYT8dxagnnqnJo2v8YcxRbZMF3HSP
-   Si empieza por bc1: bc1q62szs47xypu3huefwnsl02884zkphxcf3z6kgx

Se debe usar la funcionalidad de copiar y pegar ya que si se envía bitcoin a una dirección que no existe este ***no se podrá recuperar***. Como recomendación, después de pegar la dirección siempre se deben verificar los primeros 4/6 caracteres y los últimos 4/6 caracteres por seguridad.

Un ejemplo de cómo debería mandar la direccion a alguien seria asi:

-   Mi dirección btc es:
-   3KqyQBYT8dxagnnqnJo2v8YcxRbZMF3HSP
-   Empieza en 3KqyQB y termina en MF3HSP

Enviar la dirección en un mensaje independiente facilita que el receptor pueda copiar y pegar en su wallet sin hacer modificaciones (posibles errores) y al enviar como empieza y termina le permite validar que tanto el inicio como el fin de la dirección estén correctos.


## Transferencias

En la wallet busca el menú **Enviar**, **Transferir** o **Retirar**, la wallet solicitará la cantidad que deseas enviar, la dirección a la que lo vas a enviar y el costo (fee).

Ten en cuenta lo siguiente:

- Cantidad
  - Verificar que la unidad sea BTC, algunas wallets usan una unidad diferente por defecto. Puedes verificar las diferentes unidades en [Bitcoin units](https://en.bitcoin.it/wiki/Units){:target="_blank"}.
  - Por lo general los decimales se separan con punto (.), así que verifica como lo usa tu wallet antes de ingresar la cantidad.
  - Si estás pagando un servicio usa el botón/funcionalidad de copiar y pegar, ya que algunas cantidades pueden tener muchos decimales y por lo general debes pagar la cantidad exacta.
  - Verifica si tu wallet descuenta el fee de la cantidad o si lo suma, esto afectará tu balance y el total enviado por lo que podrías tener problemas si estas pagando un servicio que requiere un valor exacto. Por lo general las wallets permiten validar la información antes de enviar la transacción a la red.

- Dirección
  - Verifica que sea una dirección btc válida.
  - Como ya lo mencionamos, debe empezar por 1, 3 o bc1.
  - Copia y pega siempre la dirección. NO LA DIGITES.
  - Siempre verifica los primeros 4/6 caracteres y los últimos 4/6 caracteres.
  - Si tienes dudas puedes verificar si es una dirección válida [aquí](https://awebanalysis.com/en/bitcoin-address-validate/){:target="_blank"}.

- Costo (Fee): Este es uno de los elementos que genera más problemas a la hora de enviar bitcoin. Si no lo configuras correctamente tu transacción podría demorar hasta días en ser confirmada por lo que debes tener en cuenta lo siguiente:

  - Si estás usando la wallet de un exchange, estos definen sus propios costos (fees). Verificalos antes de usarlos ya que pueden ser variables.
  - La unidad que se usa para determinarlo es **Satoshis/vByte**.
  - Puedes ver un valor sugerido de acuerdo al tiempo requerido de confirmacion en: [Bitcoinfees.net](https://bitcoinfees.net/){:target="_blank"}.
  - Si estás enviando una transacción urgente siempre usa el valor más alto.
  - Si estás enviando una cantidad baja de bitcoin ten en cuenta el costo total en btc (generalmente en la vista de confirmación que muestra la wallet) ya que puede ser más costoso que la misma cantidad que estás enviando.
  - Algunas wallets muestran un menú con valores como prioridad **Alta**, **media** o **baja**, esto realmente configura el valor del costo (fee) de transacción en **Satoshis/vByte** de acuerdo a valores ponderados de las últimas transacciones, es decir, muchas veces no es preciso y por eso siempre es recomendado que verifiques dicho valor en [Bitcoinfees.net](https://bitcoinfees.net/){:target="_blank"}.

Finalmente, algunas wallets piden otros datos como descripción o anotaciones, estos no son requeridos y no son datos que van a quedar registrados dentro de la red Bitcoin, es decir, no pueden ser vistos por terceros y solo se usan como referencia para el usuario.

Y recuerda, siempre realiza una doble verificación de todos los valores en la página/vista de confirmación de la wallet antes de enviar la transacción a la red.
