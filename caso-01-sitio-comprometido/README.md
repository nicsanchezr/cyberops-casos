# Caso 01 · Sitio web comprometido y servidor bajo ataque

Un equipo Windows navega a un sitio WordPress comprometido y es redirigido a un kit de explotación. En paralelo, el servidor web de la empresa ficticia **SEES** registra fuerza bruta SSH y solicitudes web sospechosas.

```
formaA/  caso_formaA.pcap.zip   auth.log   access.log
formaB/  caso_formaB.pcap.zip   auth.log   access.log
SHA256SUMS.txt
```

## Uso

```
sha256sum -c SHA256SUMS.txt
cd formaA                      # o formaB, según la forma asignada
unzip -P infected caso_formaA.pcap.zip
```

Contraseña de los zip: `infected`

Herramientas sugeridas: Wireshark, NetworkMiner, tcpdump, tshark, Zeek y comandos nativos de Linux (`grep`, `awk`, `sort`, `uniq`).

## Fuentes

| Forma | Captura | Fuente original |
|---|---|---|
| A | `2014-11-16-traffic-analysis-exercise.pcap` | https://www.malware-traffic-analysis.net/2014/11/16/index.html |
| B | `2015-02-15-traffic-analysis-exercise.pcap` | https://www.malware-traffic-analysis.net/2015/02/15/index.html |

Las capturas son ejercicios de análisis de tráfico publicados por Brad Duncan en malware-traffic-analysis.net.

Los archivos `auth.log` y `access.log` son **simulados**. Las direcciones IP externas pertenecen a rangos reservados para documentación (RFC 5737: 192.0.2.0/24, 198.51.100.0/24, 203.0.113.0/24) y no corresponden a sistemas reales.
