<div align="center">
  <img src="https://axys.fabrictd.com/assets/instalador.png" alt="Axys Logo" width="150"/>
  <h1>Axys ERP - Release Storage</h1>
  <p><strong>Repositorio Oficial de Binarios y Distribuciones (Production Releases)</strong></p>
</div>

<hr>

## 📦 Acerca de este repositorio

Este repositorio opera exclusivamente como el **Storage de Binarios Oficiales** para las versiones compiladas de **Axys ERP**. Aquí se alojan los instaladores `.exe` de producción que luego son distribuidos a los clientes a través del sitio web oficial: [Axys.fabrictd.com](https://axys.fabrictd.com).

> ⚠️ **ATENCIÓN:** Este repositorio **NO** contiene el código fuente de Axys ERP. Es de uso exclusivo para alojamiento de _releases_ (binarios, setups y parches de actualización) gestionados mediante Continuous Delivery y automatización por el Bot de Lanzamientos interno.

## 🚀 Arquitecturas Distribuidas

Los binarios subidos aquí cubren las versiones oficiales del ecosistema:

* **Axys Ones (`Stand-Alone`):** Instalador que despliega el software con motor SQLite nativo para ejecución en una única terminal (Punto de Venta o Administración aislada).
* **Axys Sync (`Client/Server`):** Instalador diseñado para topologías de red local (LAN) operando contra un servidor centralizado MySQL / MariaDB (ej. vía XAMPP).

## 🔐 Integridad Criptográfica (SHA-256)

Para garantizar la seguridad corporativa y la integridad del software contra manipulaciones, cada Release generado viene acompañado de un hash **SHA-256**.
Los hashes son publicados directamente en la web oficial en el historial de actualizaciones. Los clientes pueden verificar la integridad del `.exe` descargado contrastándolo con el hash público usando PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 .\Axys_Setup_vX.X.X.exe
```

---
<div align="center">
  <i>© 2026 Axys Software. Todos los derechos reservados.</i><br>
  <i>Desarrollado y mantenido por <b><a href="https://www.fabrictd.com">FabriCTD</a></b></i>
</div>
