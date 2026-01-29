# EVPN-BGP-VxLAN
## Topologia del Laboratorio
![Topología](BGP_EVPN_VxLAN/img_1.png)

## SESIONES EVPN BGP LEAFs

![1](BGP_EVPN_VxLAN/img_21.png)
![1](BGP_EVPN_VxLAN/img_22.png)
![1](BGP_EVPN_VxLAN/img_23.png)

1 - show bgp evpn summary
Estas imagenes muestran el estado general del control-plane EVPN mediante BGP.
Se observa que las sesiones BGP EVPN están establecidas correctamente entre los dispositivos (Leaf, Spine y Border Leaf), confirmando conectividad del overlay EVPN.

Los contadores de prefijos recibidos validan que:
EVPN está intercambiando información de forma activa
Los Route Reflectors (Spines) están funcionando correctamente
Los Border Leafs reciben y anuncian rutas EVPN inter-DC

2 - show bgp evpn instance
Adicionalmente estas imagenes muestran las instancias EVPN activas, asociando:

VLANs
VNIs
RT-RD
Se valida que:
Cada VLAN está correctamente mapeada a su VNI
El diseño lógico del overlay coincide con la arquitectura planeada

