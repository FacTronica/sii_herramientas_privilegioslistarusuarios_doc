::: {align="center"}
# 🚀 API Factronica SII Chile

### Integración directa con el Servicio de Impuestos Internos para sistemas de Factura Electrónica

```{=html}
<p>
```
API profesional para consultar usuarios autorizados y privilegios SII
Chile mediante integración REST JSON.
```{=html}
</p>
```
`<br>`{=html}

`<img src="https://img.shields.io/badge/API-REST-blue?style=for-the-badge">`{=html}
`<img src="https://img.shields.io/badge/SII-Chile-red?style=for-the-badge">`{=html}
`<img src="https://img.shields.io/badge/JSON-Integration-green?style=for-the-badge">`{=html}
:::

------------------------------------------------------------------------

## 📖 Descripción

**API Factronica - Listar Usuarios con Privilegios SII Chile** permite
integrar sistemas propios con el ecosistema tributario chileno para
consultar usuarios autorizados dentro del SII.

Pensada para integradores, desarrolladores y empresas que necesitan
automatizar procesos relacionados con:

-   Factura Electrónica
-   Boleta Electrónica
-   Auditorías tributarias
-   Validación de permisos
-   Sistemas ERP

------------------------------------------------------------------------

# ⚡ Características principales

```{=html}
<table>
```
```{=html}
<tr>
```
```{=html}
<td width="50%">
```
### 🔐 Seguridad

-   Comunicación HTTPS
-   Uso de Token API
-   Control de acceso
-   Procesos auditables

```{=html}
</td>
```
```{=html}
<td width="50%">
```
### 🚀 Integración

-   API REST
-   Peticiones JSON
-   Respuestas estructuradas
-   Compatible con cualquier lenguaje

```{=html}
</td>
```
```{=html}
</tr>
```
```{=html}
<tr>
```
```{=html}
<td>
```
### 🏢 Ambientes SII

✅ Certificación\
✅ Producción

```{=html}
</td>
```
```{=html}
<td>
```
### 🧩 Compatible

PHP\
Node.js\
Java\
Python\
.NET

```{=html}
</td>
```
```{=html}
</tr>
```
```{=html}
</table>
```

------------------------------------------------------------------------

# 💼 Modalidades disponibles

## 🖥️ API SDK - Instalación propia

Para empresas que desean controlar completamente su infraestructura.

Incluye:

✅ Código fuente\
✅ Instalación en servidor propio\
✅ Personalización\
✅ Independencia de proveedores externos

### Precio

    $100.000 + IVA
    Pago único

------------------------------------------------------------------------

## ☁️ API SaaS - Servicio administrado

Utiliza la API sin preocuparte de servidores ni actualizaciones.

Incluye:

✅ Acceso Suite API Factronica\
✅ Actualizaciones permanentes\
✅ Nuevas funcionalidades\
✅ Servicio administrado

### Precio

    1 UF mensual

------------------------------------------------------------------------

# 🔄 Flujo de integración

``` text
Sistema Cliente

      |
      v

API Factronica

      |
      v

SII Chile
```

------------------------------------------------------------------------

# 📌 Crear petición JSON

``` json
{
  "TOKEN": "-token-api-",
  "RUT": "-rut-empresa-",
  "Clave": "-clave-sii-",
  "Periodo": "202602",
  "CodTipoDoc": "3941"
}
```

------------------------------------------------------------------------

# 📡 Ejecutar consulta API

Ejemplo CURL:

``` bash
curl -X POST \
"https://dev.factronica.cl/api/sii_herramientas_boletaobtenerlistado/index.php" \
-H "Content-Type: application/json" \
-d '
{
 "token_api":"API_KEY",
 "rutpyme":"11111111",
 "rutpyme_dv":"1"
}'
```

------------------------------------------------------------------------

# 📥 Respuesta API

``` json
{
 "codigo":200,
 "estado":"OK",
 "token":"ABC123",
 "datos":[
   {
    "rut":"11111111-2",
    "nombre":"USUARIO DEMO",
    "administrador":"S",
    "firmar_documentos":"S",
    "consulta":"S"
   }
 ]
}
```

------------------------------------------------------------------------

# 🎯 Casos de uso

  Cliente             Uso
  ------------------- ---------------------------
  ERP                 Sincronización automática
  Software Contable   Validación usuarios
  Integradores        Crear soluciones SII
  Empresas            Control interno

------------------------------------------------------------------------

# 🌎 Ambientes

  Ambiente   Descripción
  ---------- -------------------
  Maullín    Certificación SII
  Palena     Producción SII

------------------------------------------------------------------------

# 🛠️ Requisitos

-   Acceso API Factronica
-   Credenciales SII válidas
-   Servidor con salida HTTPS
-   Cliente HTTP

------------------------------------------------------------------------

::: {align="center"}
## Factronica API Suite

Construyendo integraciones modernas con SII Chile 🇨🇱
:::
