# 🚀 API Factronica - Listar Usuarios con Privilegios SII Chile

```{=html}
<p align="center">
```
`<b>`{=html}API para integración con SII Chile Factura
Electrónica`</b>`{=html}`<br>`{=html} Consulta usuarios autorizados y
privilegios asociados en ambientes SII.
```{=html}
</p>
```

------------------------------------------------------------------------

## 📌 Descripción

**API Factronica - Listar Usuarios con Privilegios SII Chile** permite
consultar los usuarios que poseen permisos configurados en el **Servicio
de Impuestos Internos (SII Chile)** para operar con documentos
tributarios electrónicos.

Pensada para:

-   Integradores de sistemas
-   Empresas con software propio
-   Desarrolladores
-   Sistemas ERP / Facturación electrónica
-   Automatización de procesos tributarios

------------------------------------------------------------------------

## ✨ Características

✅ Consulta usuarios autorizados SII\
✅ Compatible con ambiente certificación y producción\
✅ Integración mediante JSON API\
✅ Respuestas estructuradas en JSON\
✅ Fácil integración con PHP, Node.js, Java, Python y cualquier lenguaje
compatible con HTTP

------------------------------------------------------------------------

# 💰 Modalidades

## API SDK - Pago Único

Ideal para integradores que necesitan instalar la API en sus propios
servidores.

Incluye:

-   Código fuente API
-   Personalización según procesos propios
-   Control total de infraestructura
-   Sin límites de consultas dependiendo del servidor propio
-   Posibilidad de ofrecer servicio API a clientes finales

Valor referencial:

    $100.000 + IVA Pago Único

------------------------------------------------------------------------

## API SaaS - Servicio Mensual

Usa la API como servicio sin preocuparse por instalación ni
mantenimiento.

Incluye:

-   Acceso a la Suite API Factronica
-   Actualizaciones permanentes
-   Nuevas funcionalidades
-   Disponibilidad administrada

Valor referencial:

    1 UF mensual

------------------------------------------------------------------------

# 🌎 Ambientes soportados

  Ambiente   Uso
  ---------- -------------------------
  Maullín    Certificación SII Chile
  Palena     Producción SII Chile

------------------------------------------------------------------------

# 🔄 Flujo de integración

1.  Crear petición JSON
2.  Enviar petición HTTP POST
3.  Recibir respuesta API
4.  Procesar información obtenida

------------------------------------------------------------------------

# 1) Crear petición JSON

Ejemplo:

``` json
{
  "TOKEN": "-token-acceso-api-",
  "RUT": "-rut-empresa-",
  "Clave": "-clave-sii-empresa",
  "Periodo": "202602",
  "CodTipoDoc": "3941"
}
```

------------------------------------------------------------------------

# 2) Enviar petición

Ejemplo utilizando CURL:

``` bash
curl -X POST "https://dev.factronica.cl/api/sii_herramientas_boletaobtenerlistado/index.php" \
-H "Content-Type: application/json" \
-d '
{
  "token_api":"su-api-key",
  "rutpyme":"11111111",
  "rutpyme_dv":"1",
  "rutcertificado":"22222222",
  "rutcertificado_dv":"2",
  "certificado_clave":"clave-certificado",
  "certificado_llavepublica":"llave-publica-pem",
  "certificado_llaveprivada":"llave-privada-pem"
}'
```

También puedes enviar un archivo JSON:

``` bash
curl -X POST "URL_API" \
-H "Content-Type: application/json" \
-d @datos_json.json
```

------------------------------------------------------------------------

# 3) Respuesta API

Ejemplo respuesta exitosa:

``` json
{
  "codigo":200,
  "estado":"OK",
  "token":"2F92FOHS3NHSX",
  "datos":[
    {
      "rut":"11111111-2",
      "nombre":"PEDRO PICAPIEDRAS",
      "administrador":"S",
      "solicitar_folios":"S",
      "anular_folios":"S",
      "firmar_documentos":"S",
      "enviar_documentos":"S",
      "consulta":"S"
    }
  ]
}
```

------------------------------------------------------------------------

# 🧩 Casos de uso

-   Validar usuarios autorizados antes de emitir documentos
-   Sincronizar permisos SII con sistemas internos
-   Auditoría tributaria
-   Integraciones ERP
-   Plataformas de facturación electrónica

------------------------------------------------------------------------

# 🏗️ Arquitectura recomendada

    Sistema Cliente
           |
           |
           v
    API Factronica
           |
           |
           v
    SII Chile

------------------------------------------------------------------------

# 🔐 Seguridad

Recomendaciones:

-   Mantener protegido el token API
-   No publicar credenciales SII
-   Usar HTTPS
-   Registrar logs de integración
-   Controlar acceso por aplicación

------------------------------------------------------------------------

# 📞 Soporte

Proyecto desarrollado por **Factronica**.

Repositorio:

https://github.com/FacTronica

------------------------------------------------------------------------

```{=html}
<p align="center">
```
Made with ❤️ para integraciones SII Chile
```{=html}
</p>
```
