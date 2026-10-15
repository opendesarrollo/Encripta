<div align="left">
  <pre style="font-family: monospace; line-height: 1.1; overflow-x: auto;">
███████╗███╗   ██╗ ██████╗██████╗ ██╗██████╗ ████████╗ █████╗
██╔════╝████╗  ██║██╔════╝██╔══██╗██║██╔══██╗╚══██╔══╝██╔══██╗
█████╗  ██╔██╗ ██║██║     ██████╔╝██║██████╔╝   ██║   ███████║
██╔══╝  ██║╚██╗██║██║     ██╔══██╗██║██╔═══╝    ██║   ██╔══██║
███████╗██║ ╚████║╚██████╗██║  ██║██║██║        ██║   ██║  ██║
╚══════╝╚═╝  ╚═══╝ ╚═════╝╚═╝  ╚═╝╚═╝╚═╝        ╚═╝   ╚═╝  ╚═╝
  </pre>
</div>

### Tu información. Tus decisiones. Tu control.

**Protege tus mensajes y comparte información confidencial de forma sencilla, privada y sin complicaciones.**

Encripta es una aplicación de escritorio que permite cifrar y descifrar mensajes mediante claves públicas y privadas. Está diseñada para que cualquier persona pueda proteger su información, sin necesidad de tener conocimientos avanzados de informática o seguridad digital.

Tu información se procesa directamente en tu dispositivo, sin necesidad de enviarla a servidores externos.

**[Descargar Encripta](https://github.com/opendesarrollo/Encripta/releases) | [Consultar documentación](#documentación)**

---

## ¿Por qué utilizar Encripta?

Cada día compartimos información personal, laboral y confidencial a través de correos electrónicos, aplicaciones de mensajería y otros medios digitales.

Pero ¿qué sucede cuando esa información llega a manos equivocadas?

**Encripta te permite proteger el contenido de tus mensajes antes de compartirlos.**

- **Protege tus mensajes:** convierte información legible en contenido cifrado.
- **Mantén el control:** tú decides con quién compartir la información.
- **Funciona sin Internet:** cifra y descifra directamente en tu dispositivo.
- **Comparte con facilidad:** envía archivos protegidos mediante WhatsApp, correo electrónico u otros medios.
- **Sin cuentas obligatorias:** no necesitas registrarte ni proporcionar información personal para utilizarlo.

## ¿Qué puedes hacer con Encripta?

Actualmente, Encripta permite proteger mensajes utilizando un sistema de claves públicas y privadas.

### Crear tus propias claves

Genera dos claves relacionadas entre sí: una pública, que puedes compartir, y otra privada, que debes mantener protegida.

### Cifrar mensajes

Escribe un mensaje, selecciona la clave pública del destinatario y genera un archivo protegido.

### Descifrar mensajes

Recupera el contenido de los mensajes que recibas utilizando tu clave privada y contraseña.

### Compartir información protegida

Envía los archivos cifrados a otras personas mediante tus medios de comunicación habituales.

---

## Dos formas de utilizar Encripta

Encripta está disponible en dos modalidades para adaptarse a diferentes necesidades.

### Encripta Desktop — Interfaz gráfica

**La forma más sencilla de proteger tus mensajes.**

Utiliza una interfaz visual para crear claves, cifrar mensajes y recuperar información protegida, sin necesidad de escribir comandos.

**Ideal para:** personas que buscan una experiencia sencilla y visual.

[Consultar manual de Encripta Desktop](docs/gui/cifrado-asimetrico.md)

### Encripta CLI — Línea de comandos

**Protege tu información directamente desde la terminal.**

Permite realizar operaciones de cifrado y descifrado mediante instrucciones sencillas.

**Ideal para:** usuarios familiarizados con la terminal, desarrolladores y administradores de sistemas.

[Consultar manual de Encripta CLI](docs/cli/cifrado-asimetrico.md)

---

## ¿Cómo funciona?

Imagina que deseas enviar un mensaje privado a otra persona.

**Paso 1. Crear las claves**

El destinatario utiliza Encripta para generar su clave pública y su clave privada.

**Paso 2. Compartir la clave pública**

El destinatario comparte contigo su clave pública. Su clave privada permanece protegida.

**Paso 3. Proteger el mensaje**

Escribes el mensaje y lo cifras utilizando la clave pública del destinatario.

**Paso 4. Enviar el archivo cifrado**

Puedes compartir el archivo generado por WhatsApp, correo electrónico u otro medio.

**Paso 5. Recuperar el mensaje**

El destinatario utiliza su clave privada y contraseña para descifrar el archivo y leer el mensaje original.

**No necesitas compartir contraseñas ni claves privadas para intercambiar mensajes protegidos.**

---

## Descargar Encripta

Obtén las versiones disponibles desde el repositorio oficial de OpenDesarrollo.

### [Descargar la última versión de Encripta](https://github.com/opendesarrollo/Encripta/releases/latest)

Para comenzar:

1. Accede a la sección de descargas.
2. Selecciona la versión compatible con tu sistema operativo.
3. Descarga el ejecutable correspondiente.
4. Abre Encripta y comienza a proteger tus mensajes.

**Recomendación:** si no estás familiarizado con la terminal, utiliza Encripta Desktop.

---

## Documentación

¿Es tu primera vez utilizando Encripta?

Preparamos guías sencillas para acompañarte desde la creación de tus primeras claves hasta el intercambio de mensajes protegidos.

| Modalidad | Manual de usuario |
|---|---|
| Interfaz gráfica (Desktop) | [Cifrado asimétrico](docs/gui/cifrado-asimetrico.md) |
| Línea de comandos (CLI) | [Cifrado asimétrico](docs/cli/cifrado-asimetrico.md) |

Los manuales incluyen instrucciones paso a paso, ejemplos prácticos y recomendaciones para proteger tu información.

---

## Tu privacidad es importante

Encripta está desarrollado bajo tres principios fundamentales.

### Privacidad por diseño

La información se procesa localmente en tu dispositivo, sin enviarse a servidores de OpenDesarrollo para realizar las operaciones de cifrado y descifrado.

### Control personal

Tú decides qué información proteger, qué claves utilizar y con quién compartir tus mensajes cifrados.

### Independencia

No necesitas crear una cuenta ni depender de servicios externos para cifrar o descifrar tus mensajes.

La protección de tus claves privadas, contraseñas y dispositivos sigue siendo fundamental para mantener segura tu información.

---

## Preguntas frecuentes

### ¿Necesito conocimientos técnicos para utilizar Encripta?

No. Encripta Desktop ofrece una interfaz gráfica diseñada para facilitar la protección de mensajes.

### ¿Encripta necesita conexión a Internet?

No para cifrar o descifrar mensajes. Estas operaciones se realizan directamente en tu dispositivo.

### ¿Puedo compartir mensajes cifrados por WhatsApp?

Sí. Puedes enviar los archivos protegidos como documentos mediante WhatsApp, correo electrónico u otras aplicaciones.

### ¿Puedo compartir mi clave pública?

Sí. Tu clave pública puede compartirse con otras personas para que puedan enviarte mensajes protegidos.

### ¿Puedo compartir mi clave privada?

No. Tu clave privada debe permanecer bajo tu control. También debes proteger la contraseña utilizada para acceder a ella.

### ¿Qué sucede si pierdo mi clave privada?

Si no conservas un respaldo, podrías perder definitivamente el acceso a los mensajes cifrados para esa clave.

### ¿Encripta es de código abierto?

No. Encripta es un software de código fuente privado. Este repositorio público está destinado a distribuir sus versiones ejecutables, documentación y actualizaciones.

---

## Nuestra misión

Hacer que la protección de información sea accesible para cualquier persona, ofreciendo herramientas sencillas que permitan mantener el control sobre la privacidad de sus datos.

## Nuestra visión

Contribuir a un entorno digital en el que proteger información personal y confidencial sea una práctica cotidiana, accesible e independiente.

---

## Actualizaciones y nuevas funcionalidades

Encripta es un proyecto en evolución.

Continuaremos incorporando mejoras y nuevas funcionalidades orientadas a facilitar la protección de información.

Puedes consultar las versiones disponibles, novedades y actualizaciones en:

[Ver versiones y actualizaciones](https://github.com/opendesarrollo/Encripta/releases)

## Reportar problemas o sugerir mejoras

Tu experiencia nos ayuda a mejorar Encripta.

Si encuentras algún problema o deseas proponer una nueva funcionalidad, puedes comunicarlo mediante el repositorio oficial.

[Reportar un problema o sugerir una mejora](https://github.com/opendesarrollo/Encripta/issues)

No incluyas contraseñas, claves privadas ni información confidencial en tus reportes.

---

## Información del proyecto

**Nombre:** Encripta  
**Desarrollador:** OpenDesarrollo  
**Modalidades:** Desktop y CLI  
**Distribución:** Ejecutables de código fuente privado  
**Repositorio oficial:** https://github.com/opendesarrollo/Encripta

© 2026 OpenDesarrollo. Todos los derechos reservados.

---

### Tu información merece protección.

**Encripta — Tu información. Tus decisiones. Tu control.**
