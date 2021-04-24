# XDV Facturacion Electronica para PAC (Proveedor Autorizados Calificados)

**XDV para PAC** o **Red XDV PAC/XDV PAC Network** es una solucion decentralizada de consorcio que utiliza IPFS, IPLD y Carteras Criptograficas y  una combinacion de agentes y sistemas de sincronizacion para administrar confeccion, generacion, firmado y envios de mensajes con contenido de facturas electronicas.

Features incluyeen:


- **IPLD storage and query**: Allows for document patching and query with IPLD
- **DID  Ethereum compatible**: Uses did-ethr for identity
- **API or JSON-RPC**: Use web3 or API to integrate to protocol
- **Built-in NFT Tokenization**
- **XmlDsig Validation API**
- **XDV integration**
- **Proxy Re Encryption or DF Key Exchange (Noise Protocol)**


## Architecture Design V1

![Sequence diagram](https://github.com/Electronic-Signatures-Industries/xdv-invoice-protocol/blob/main/archdesign.png)

## Architecture Design V2 - PAC Network

Una red XDV PAC consiste de uno o mas clusteres `IPFS` en modo privado, un PAC puede operar un cluster privado por su cuenta o unirse a otros nodos privados XDV PAC en modo consorcio. El beneficio que se obtiene para una PAC en modo consorcio con `IPFS` para sus cuentahabientes son la disponibilidad de las facturas, y menor costos de operacion, ya que el consorcio abarata los costos de sincronizacion bridge entre la red XDV PAC y los sistemas del DGI.

Un sistema decentralizado con `IPFS` y usando `IPLD` como `Merkle Tree` o `Merkle Forest` tienen, ademas de ser almacenamiento por hashes criptograficos, beneficios en la replicacion de datos ya que utiliza `libp2p`, lo cual permite subscripciones de eventos. Este ultimo punto importante, ya que podemos crear un bridge o puente entre XDV PAC y DGI y obtener eventos bidireccionales, lo cual permite crear agentes en tiempo real de cualquier evento ocurrido de una factura en  particular.

Opcionalmente, facturas sincronizadas con DGI y que requieran ser convertidas a otros instrumentos financieros, pueden optar por el puente de Tokenizacion de Activos, el cual en una version 3 de la red, permitira tokenizar facturas como factoring y estas intercambiarse en mercados de finanzas digitales (DeFi).

## Reference Implementation

TODO

## Protocol Fees

Planteamos los fees del protocolo del siguiente modo:

- Anualidad y Precios por Facturas
- (Opcional) Trazabilidad sincronizada a blockchain publico o privado
- (Opcional) Tokenizacion de Activos
- (Opcional) Encriptacion

## Commercial inquiry

`info@ifesa.tech`
