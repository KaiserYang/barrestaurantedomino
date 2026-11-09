# Bar Restaurante Domino

Sitio web estático y multipágina de Bar Restaurante Domino, en Las Tablas (Madrid).

## Páginas públicas

- `index.html`: portada, platos destacados, menú del día, planes, horario y ubicación.
- `desayunos.html`: desayunos, bebidas, sándwiches, hamburguesas, platos combinados y bocadillos.
- `raciones.html`: raciones de la casa, tapas y pinchos.
- `carta-vinos.html`: vinos y bebidas.
- `reservas.html`: reservas por WhatsApp o llamada.
- `contacto.html`: contacto y mapa.
- `aviso-legal.html`, `privacidad.html`, `cookies.html`: información legal.

## Estructura

- `assets/css/styles.css`: estilos compartidos y portada.
- `assets/js/main.js`: navegación responsive, submenús y presentación de precios.
- `Resources/`: logotipo, fotografías y fondos de las cartas.

No requiere compilación: puede servirse directamente como sitio estático.

## Menú del día (Google Docs)

`menu-del-dia.html` usa la cabecera, pie y navegación compartidos. Sus estilos adicionales están en `assets/css/menu-del-dia.css`.

Configuración inicial:
1. En Google Docs: Archivo > Compartir > Publicar en la Web > Insertar.
2. Activar la republicación automática de cambios.
3. Copiar la URL del `src` del iframe de Google (`https://docs.google.com/document/d/e/.../pub?embedded=true`).
4. En el iframe de `menu-del-dia.html`, sustituir `src="about:blank"` por esa URL y eliminar TODO el atributo `srcdoc`. Si se conserva `srcdoc`, este prevalece sobre `src`.

Hasta conectar el documento, aparece un aviso para consultar el menú por teléfono. No se muestran platos inventados.

Para actualizar: editar el mismo documento de Google Docs, poniendo fecha, platos, precio y qué incluye. No hay que editar el HTML. El contenido publicado es público; no incluir información privada. El precio exterior de 15 euros es fijo y debe actualizarse en el HTML si cambia. El iframe tiene desplazamiento propio para documentos largos; no se puede ajustar su altura desde la web leyendo el contenido de Google por las restricciones entre dominios.
