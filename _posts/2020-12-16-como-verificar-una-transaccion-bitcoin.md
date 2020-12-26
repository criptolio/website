---
layout: post
title:  "¿Cómo verificar una transacción bitcoin?"
author: jp
categories: [ básico ]
image: assets/images/bitcoin/verificar-transaccion-bitcoin.jpg
featured: false
hidden: false
---


Una vez hayas realizado una [transferencia]({% post_url 2020-12-15-como-hacer-un-deposito-o-transferencia-en-bitcoin %}) o te hayan [depositado]({% post_url 2020-12-15-como-hacer-un-deposito-o-transferencia-en-bitcoin %}) bitcoin debes verificar dos cosas:

1.  Que la transacción efectivamente haya sido enviada (sea visible) en la red Bitcoin, y...
2.  Una vez verificado lo anterior, debes verificar si la transacción ha sido completada (confirmada).

## ¿Cómo verificar si la transacción ya fue enviada?

Al realizar una transacción, tu [wallet]({% post_url 2020-12-14-que-es-un-wallet-bitcoin %}) o la de la persona o servicio que lo envía, mostrará un código de confirmación (transaction id, transaction hash, hash o tx Hash) que es similar al número de comprobante que recibes al realizar una transacción en un banco tradicional.

Existen múltiples páginas web, exploradores de la red Bitcoin, en las que puedes consultar el estado de una transacción con dicho comprobante o con la dirección de destino.

-   [Blockonomics.co](https://www.blockonomics.co/){:target="_blank"}
-   [Blockchair.com](https://blockchair.com/){:target="_blank"}
-   [Btc.com](https://btc.com/){:target="_blank"}
-   [Blockchain.com](https://www.blockchain.com/){:target="_blank"}
-   Otros: puedes buscar en google [“bitcoin blockchain explorer”](https://www.google.com/search?q=bitcoin+blockchain+explorer){:target="_blank"}

Debes tener en cuenta que algunos [exchanges]({% post_url 2020-12-18-donde-se-puede-comprar-vender-bitcoin %}), no procesan las transacciones inmediatamente por lo que hay un retraso, generalmente 15 minutos, hasta que envían las transacciones a la red. Debes esperar hasta que el exchange te muestre el comprobante (Tx Hash) para poder verificarlo.

En estos exploradores encontrarás un cuadro de búsqueda en la que puedes pegar tu comprobante (Tx hash) o la dirección de destino y al dar enter o buscar, te mostrará una información similar a lo siguiente:

![Transacción bitcoin sin confirmar]({{ site.baseurl }}/assets/images/bitcoin/bitcoin-transaction-sin-confirmar.png)

![Transacción bitcoin confirmada]({{ site.baseurl }}/assets/images/bitcoin/bitcoin-transaction-confirmada.png)

Cada explorador presenta la misma información de forma diferente pero básicamente tienes los siguientes datos:

- **Inputs**: direcciones de origen
- **Outputs**: direcciones de destino, dentro de estas debe estar tu dirección de depósito o la dirección a la que enviaste.
- **Tx Hash**: comprobante de la transacción. Es un conjunto de números y letras similar a:
  - 2ef32711905c98c74ff9c1ec6af57fbc750daf58e1194e6aeb7572d46d5c0e3e
  - 7996563eddcbadf3b3918ab5410cb315de540e6ab43b9696e6e693790cefbf88
- **Costo (fee)**: costo de la transacción en bitcoin (BTC) o en Satoshis/vByte
- **Fecha de la transacción**: si la transacción está sin confirmar esta fecha irá cambiando hasta que se realice la primera confirmación.
- **Cantidad**: valor en bitcoin. Se puede mostrar al lado de las direcciones de destino o como resumen de la transacción (valores en recuadro verde).
- **Cantidad de confirmaciones**: si no tiene confirmaciones aparecerá ***Sin confirmar*** o ***Unconfirmed*** y cuando ya tenga confirmaciones aparecerá un número mayor o igual a 1.

Existen otros valores pero estos son los más importantes a la hora de verificar que hayas/hayan realizado la transacción correctamente.

## ¿Cómo verificar si la transacción ya fue completada (confirmada)?

Una transacción es considerada “completa” o confirmada una vez el servicio o persona a la que estés enviando considere que es imposible deshacer la transacción.

Teóricamente si una transacción tiene 6 confirmaciones en la red Bitcoin es imposible deshacer la transacción, sin embargo, algunos servicios sólo requieren 3 confirmaciones y otros dependiendo del monto varían entre 1 y 6 confirmaciones. Siempre debes verificar cuantas confirmaciones requiere el servicio al que estés enviando bitcoin y revisar en el explorador el estado de tu transacción.

Pero si depositan en mi wallet **¿Cuántas confirmaciones debo esperar?** Por lo general, si los depósitos o transferencias son pequeños, con una confirmación es suficiente, pero ten en cuenta que siempre debes esperar al menos ***UNA CONFIRMACIÓN*** en la red Bitcoin si estás intercambiando o vendiendo a un tercero.
