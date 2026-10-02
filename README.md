# cyberops-casos

Casos prácticos de análisis de tráfico de red, forense de red y revisión de logs para la formación de analistas CyberOps / SOC.

| Caso | Tema | Herramientas |
|---|---|---|
| [caso-01-sitio-comprometido](caso-01-sitio-comprometido/) | Sitio WordPress comprometido → kit de explotación; fuerza bruta SSH y webshell en servidor web | Wireshark, NetworkMiner, tcpdump, tshark, Zeek, CLI Linux |

Cada caso puede tener varias **formas** (A, B, …) con archivos distintos, para que cada equipo trabaje con su propio conjunto de evidencias. Use solo la forma que le fue asignada.

## ⚠ Advertencia de seguridad

Algunos casos contienen **tráfico real de infecciones de malware**. Los pcap se distribuyen dentro de zip protegidos con la contraseña `infected` para evitar que el antivirus los elimine.

- Descomprima y analice los archivos solo dentro de una máquina virtual Linux aislada.
- No ejecute ni abra los archivos que extraiga de las capturas (ejecutables, Java, Flash, documentos).
- Para consultar reputación, use solo los hashes; no suba archivos a servicios externos.

## Integridad

Cada caso incluye `SHA256SUMS.txt`. Verifique antes de trabajar:

```
sha256sum -c SHA256SUMS.txt
```

## Atribución

Las capturas de tráfico de malware provienen de [malware-traffic-analysis.net](https://www.malware-traffic-analysis.net/), de Brad Duncan, y se incluyen con fines formativos. Los derechos sobre esas capturas pertenecen a su autor. Los logs y escenarios simulados son de elaboración propia.
