# Tutorial de Instalación del Archivo de Inicio de Sesión en Mikrotik

## Requisitos Previos
- Acceso al router Mikrotik.
- Conexión a Internet.
- Archivo de inicio de sesión personalizado.
- Winbox instalado en tu computadora.

## Pasos de Instalación

### 1. Acceder al Router Mikrotik
1. Abre Winbox en tu computadora.
2. Ingresa la dirección IP de tu router Mikrotik en el campo **Connect To**.
3. Ingresa tus credenciales de administrador en los campos **Login** y **Password**.
4. Haz clic en **Connect** para acceder al router.

### 2. Subir el Archivo de Inicio de Sesión
1. Navega a la sección **Files** en la interfaz de Mikrotik.
2. Haz clic en el botón **Upload**.
3. Selecciona el archivo de inicio de sesión personalizado desde tu computadora y súbelo.
4. Sube también las carpetas `img` y `css` que contienen los recursos necesarios.
5. Sube el archivo `login.html` y reemplaza el archivo existente. **Nota:** Haz una copia de seguridad del archivo `login.html` antiguo antes de reemplazarlo.
6. En la carpeta `img`, sustituye las imágenes `imagen1.png`, `imagen2.png`, `imagen3.png` e `imagen4.png` con el mismo nombre y extensión de formato de imagen. Las dimensiones recomendadas son 200px x 600px o al menos que tengan un aspecto rectangular. **Sugerencia:** Usa una página de compresión de imágenes como [compressor.io](https://compressor.io/) para reducir el peso de las imágenes.

### 3. Configurar el Hotspot
1. Ve a la sección **IP** y selecciona **Hotspot**.
2. Selecciona el servidor de Hotspot que deseas configurar.
3. Ve a la pestaña **Server Profiles** y selecciona el perfil que estás utilizando.
4. En la pestaña **HTML Directory**, selecciona el archivo de inicio de sesión que subiste.
5. Habilita el **Trial** en la pestaña **Login** del perfil del servidor. Configura los minutos gratuitos y el tiempo de restablecimiento para que el usuario pueda volver a habilitar el botón de probar internet.

### 4. Reiniciar el Servicio de Hotspot
1. Ve a la pestaña **Servers** en la sección **Hotspot**.
2. Selecciona el servidor de Hotspot y haz clic en **Disable**.
3. Luego, haz clic en **Enable** para reiniciar el servicio.

## Verificación
1. Desconéctate y vuelve a conectarte a la red Wi-Fi del Hotspot.
2. Deberías ver la nueva página de inicio de sesión personalizada.

¡Y eso es todo! Has instalado exitosamente el archivo de inicio de sesión en tu router Mikrotik.
