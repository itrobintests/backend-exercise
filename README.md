# El restaurante

Un famoso restaurante requiere implementar un sistema que le permita gestionar los pedidos que recibe y sus cobros.

El encargado del restaurante comenta que el restaurante sólo ofrece 6 platos distintos, a saber: ensalada caesar, risoto de hongos portobello, lasagna, carne al horno, hamburguesa de lentejas, arroz con calamares. Todos los platos se ofrecen con guarnición. El encargado no descarta la idea de agregar o cambiar platos a futuro.

De cada plato se conoce su nombre y precio.

El encargado también nos cuenta la forma de obtener el precio de cada pedido. Si bien el restaurante está abierto casi todo el día, sólo acepta pedidos 2 veces al día, por lo que maneja 2 turnos: diurno y nocturno. A futuro se piensa en disponer de más turnos.

Para calcular el precio de un pedido el encargado tiene en cuenta lo siguiente:

| Concepto/Turno         | Diurno | Nocturno |
| ---------------------- |:------:|:--------:|
| Es cliente             | 7%     | 5%       |
| Lugar de entrega < 1Km | 1%     | 1%       |
| Cantidad de Platos > 3 | 2%     | 1%       |

Salvo en el caso de que sea cliente, los porcentajes deben sumarse. Por ejemplo, considerando el caso diurno, si el pedido lo realiza una persona que no es cliente y el pedido hay que llevarlo a 2 cuadras del restaurante (200m) se le aplica sobre el total un 1% de descuento. Ahora bien, si el pedido lo realiza una persona que no es cliente y el pedido hay que llevarlo a 2 cuadras del restaurante (200m) y pidió 4 platos, entonces el descuento que se aplica es de 3% (1% + 2%).

Tener en cuenta que el restaurante recibe pedidos de personas que no forman parte de su listado de clientes.

Finalmente, el precio de un pedido se obtiene sumando el precio de cada plato. Los descuentos se aplican sobre el total.

El encargado del restaurante debe poder cambiar el turno “Diurno” / “Nocturno” cuando lo requiera.

**Supuestos**

* Asuma que al ingresar un pedido se conoce, y por lo tanto se ingresa, la distancia desde el restaurante hasta el lugar de entrega.

## Se pide

1. Diagrama de clases de la solución. En caso de aplicar algún patrón de diseño identifíquelo y justifique su desición.

2. Desarrollar la aplicación utilizando PHP 7.x o superior.

3. Codificar la solución que permita:
   
   1. Ingresar un pedido
   
   2. Obtener el precio de un pedido
   
   3. Cambiar el turno “Diurno” / “Nocturno” 

## Consideraciones

* Proporcionar una forma de verificar que la aplicación funciona. No es necesario que tenga interfaz gráfica.

* La aplicación debe estar Dockerizada.

* Si lo considera necesario, puede agregar documentación sobre la solución.

* Puede utilizar algún framework si lo desea. Si lo hace, justifique su desición.

* No es necesario que los datos sean persistidos.


