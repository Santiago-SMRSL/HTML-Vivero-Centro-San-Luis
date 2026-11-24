# Vivero de Empresas — Centro San Luis

Sitio web institucional desarrollado en **HTML5** y **CSS3** para el proyecto del **Vivero de Empresas** de 2.º curso de Sistemas Microinformáticos y Redes (SMR) del **Centro San Luis**.

El portal reúne los servicios e infraestructura tecnológica del vivero, la documentación descargable de cada fase del proyecto (P2–P10), la presentación de la ikasempresa del equipo (**VRAura**), el plan de sostenibilidad y soluciones IoT, ofertas de empleo del sector IT y un formulario de contacto para empresas interesadas en alojarse en las instalaciones.

## Estructura de páginas

* **`index.html` (¿Qué ofrecemos?):** Página principal con portada, resumen de servicios y desarrollo técnico del vivero:
  * **P2 — Infraestructura de red:** Topología en Cisco Packet Tracer con segmentación VLAN (10–80), ACLs de aislamiento en SwitchL3, firewall Cisco ASA 5506-X con DMZ y enlace WAN al Centro San Luis.
  * **P3 y P4 — Equipamiento y almacenamiento:** Configuración de servidor Ubuntu Server 26.04 LTS, BIOS/UEFI, bastionado (PAM, UFW y KeePassXC), montaje físico con controladora BBU, RAID 10 con `mdadm` y aislamiento de 6 empresas con permisos SGID (`2770`) y ACL.
  * **P5 — Servicios de red:** Instalación y verificación de Kea DHCPv4, `vsftpd`, OpenSSH (clave pública `ed25519`), `xrdp` + XFCE4 y Apache2.
  * **Incidencias:** Registro de incidencias detectadas en el despliegue en AWS y soluciones aplicadas.
  * **P10 — Despliegue en AWS:** Comparativa cloud, arquitectura de alojamiento/backups y publicación con Apache2 en una instancia EC2.
* **`empresas.html` (Empresas — P7):** Presentación de la ikasempresa **VRAura** (misión, logotipo, vídeo promocional incrustado mediante `<iframe>`, modelo Canvas, análisis DAFO, forma jurídica S.L., financiación y plan económico).
* **`sostenibilidad.html` (Sostenibilidad — P8 y P9):** Propuesta de mejora ambiental vinculada a normas ISO y ODS, junto al análisis de sensórica y arquitectura IoT para los 6 módulos y zonas comunes.
* **`ofertas.html` (Ofertas de trabajo — P6):** Selección y comparativa de ofertas reales del sector IT (FERCHAU Spain, Minsait, IRIUM y Domestika) y resumen de la dinámica de entrevistas (*role play*).
* **`contacto.html` (Contacto):** Formulario de solicitud de alojamiento en el vivero, datos del centro e imagen de las instalaciones.

## Tecnologías y diseño

* **HTML5 semántico:** Estructura organizada mediante `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>` y `<footer>`.
* **CSS3 (hoja de estilos única):** Todos los estilos unificados en `styles/style.css` con variables CSS para la paleta corporativa (`#129995` y `#122E68`), diseño *responsive* y sin frameworks externos.
* **Documentación descargable:** Carpetas locales en `/docs/` con los informes en PDF (incluyendo entregas de ambas parejas del equipo) y el archivo de simulación `.pkt`.

## Organización del proyecto

```text
/
├── index.html
├── empresas.html
├── sostenibilidad.html
├── ofertas.html
├── contacto.html
├── styles/
│   └── style.css
├── images/
│   ├── LOGOVIVERO.svg
│   ├── LOGOVIVERO Blanco.svg
│   ├── MAIN.jpg
│   ├── img2.png
│   ├── P2.png
│   ├── imagen-vivero.png
│   └── ...
├── img/
│   └── logovraura.svg
└── docs/
    ├── P2-Infraestructura-Red.pdf
    ├── P2-Topologia-Vivero.pkt
    ├── P3-Equipamiento-Informatico.pdf
    ├── P3-Equipamiento-Informatico-p2.pdf
    ├── P3-Cuaderno-Campo.pdf
    ├── P4-Almacenamiento-Vivero.pdf
    ├── P4-Almacenamiento-Vivero-p2.pdf
    ├── P4-Cuaderno-Campo.pdf
    ├── P5-Servicios-Red.pdf
    ├── P5-Servicios-Red-p2.pdf
    ├── P6-Busqueda-Empleo-Entrevista.pdf
    ├── P6-Busqueda-Empleo-Entrevista-p2.pdf
    ├── P7-Modelo-Negocio-VRAura.pdf
    ├── P8-Sostenibilidad-Vivero.pdf
    ├── P9-Soluciones-IoT.pdf
    └── P10-Despliegue-AWS.pdf

```

## Autores

Proyecto realizado por alumnos de **2.º SMR — Centro San Luis (2026)**:

* Santiago
* Raúl
* Unax
* Jon Enaitz