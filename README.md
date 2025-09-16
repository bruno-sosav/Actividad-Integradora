# Actividad-Integradora
Actividad, grupos de 3 implementando patrones de diseño. Alen, Enzo y Bruno integrantes. 

Etapa 1: Carrito con command. 
- Clases - 
Item.cs 
Carrito.cs 
EditorCarrito.cs (invoker) 
AgregarItemCommand.cs
QuitarItemCommand.cs
SetCantidadCommand.cs
CarritoPort.cs (implementa interfaz ICarritoPort)

Etapa 2: Costos de envio con Strategy + Config (singleton) 
- Clases -
/Strategy/EnvioMoto.cs
/Strategy/EnvioCorreo.cs
/Strategy/RetiroEnTienda.cs
/Straegy/EnvioService.cs
/Singleton/ConfigManager.cs (ya existe el contrato, usarlo)

Etapa 3: Pago(factory - adapter - decorator) + Pedido ( builder - observer ) + facade
- Clases -
/Payment/IPago.cs (ya declarado en contracts. usarlo)
/Payment/PagoTarjeta.cs / PagoTransfer.cs / PagoMp.cs
/Payment/PagoFactory.cs
/Payment/MpSdkFalsa.cs / PagoAdapter.cs
/Payment/PagoConImpuesto.cs / PagoConCupon.cs
/Order/Pedido.cs / PedidoBuilder.cs
/Order/Observers/{clienteObserver, LogisticaObserver, AuditoriaObserver}.cs
/Facade/CheckoutFacade.cs
