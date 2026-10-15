# Cifrado asimétrico

**Encripta — Manual de usuario (Interfaz de línea de comandos)**

## 1. ¿Qué es el cifrado asimétrico?

El cifrado asimétrico es un método que permite proteger información para que únicamente la persona a quien está destinada pueda leerla.

Para hacerlo, Encripta utiliza dos claves relacionadas entre sí:

- **Clave pública:** puedes compartirla con cualquier persona que desee enviarte mensajes protegidos.
- **Clave privada:** es personal y debes mantenerla en secreto. Se utiliza para recuperar los mensajes que recibes.

Por ejemplo, si deseas enviar un mensaje confidencial a un amigo, necesitas su clave pública para protegerlo. Tu amigo podrá recuperar el mensaje utilizando su clave privada.

**Recuerda:** la clave pública se comparte; la clave privada se protege.

## 2. Antes de comenzar

Para utilizar esta funcionalidad necesitas disponer del ejecutable de **Encripta CLI**.

La interfaz de línea de comandos permite utilizar Encripta desde una terminal, como PowerShell, Símbolo del sistema (CMD) o una terminal de Linux.

### Consultar los comandos disponibles

Ejecuta:

```bash
encripta ayuda
```

Encripta mostrará los comandos que puedes utilizar.

| Comando | Descripción |
|---|---|
| `crear-claves` | Genera un nuevo par de claves. |
| `configurar` | Configura las claves que utilizarás. |
| `cifrar` | Cifra un mensaje y genera un archivo protegido. |
| `descifrar` | Recupera un mensaje cifrado. |
| `estado` | Muestra la configuración del sistema. |
| `ayuda` | Muestra los comandos disponibles. |
| `version` | Muestra la versión de Encripta. |

**Nota:** en los ejemplos se utiliza `encripta` como nombre del ejecutable. En Windows puedes utilizar `encripta.exe` o `.\encripta.exe`, según dónde se encuentre el archivo.

## 3. Crear tus claves

Antes de recibir mensajes cifrados, necesitas generar tus propias claves.

### Pasos

**Paso 1.** Abre una terminal en la ubicación donde tienes Encripta.

**Paso 2.** Ejecuta:

```bash
encripta crear-claves
```

**Paso 3.** Ingresa una contraseña cuando sea solicitada.

```text
CREAR CLAVES

Contraseña:
Confirmar contraseña:
```

La contraseña se utiliza para proteger tu clave privada. Mientras la escribes, Encripta mostrará asteriscos.

**Paso 4.** Confirma la contraseña.

**Paso 5.** Si ambas contraseñas coinciden, Encripta generará los archivos correspondientes.

### ¿Qué archivos obtendrás?

**Clave pública**

Es el archivo que puedes compartir con amigos, familiares o compañeros de trabajo para que puedan enviarte mensajes protegidos.

**Clave privada**

Es el archivo que utilizarás para leer los mensajes cifrados que recibas.

Los archivos generados utilizan la extensión `.seg` y sus nombres son indicados por Encripta al finalizar la operación.

**Importante:** no compartas tu clave privada ni olvides tu contraseña. Si las pierdes, podrías perder el acceso a tus mensajes.

## 4. Configurar tus claves

Antes de cifrar o descifrar mensajes, debes indicar a Encripta qué claves utilizará.

### Pasos

**Paso 1.** Ejecuta:

```bash
encripta configurar
```

**Paso 2.** Encripta solicitará dos nombres de archivo:

```text
CONFIGURAR SISTEMA

Clave pública del destinatario:
Clave privada propia:
```

**Clave pública del destinatario:** ingresa el nombre de la clave pública de la persona a quien enviarás mensajes.

**Clave privada propia:** ingresa el nombre de tu clave privada, que utilizarás para leer los mensajes recibidos.

Escribe los nombres sin la extensión `.seg`, ya que Encripta la agrega al buscar los archivos.

**Paso 3.** Al finalizar, Encripta guardará la configuración en el archivo `config.seg`.

### Consultar la configuración

Puedes revisar las claves configuradas ejecutando:

```bash
encripta estado
```

Esto permite comprobar qué clave pública del destinatario y qué clave privada propia están registradas.

**Importante:** conserva los archivos de claves en la ubicación desde la que Encripta espera leerlos.

## 5. Cifrar un mensaje

Esta función permite proteger un mensaje antes de compartirlo con otra persona.

### Pasos

**Paso 1.** Comprueba que hayas configurado la clave pública del destinatario.

Puedes verificarlo mediante:

```bash
encripta estado
```

**Paso 2.** Ejecuta:

```bash
encripta cifrar
```

También puedes utilizar su comando abreviado:

```bash
encripta c
```

**Paso 3.** Encripta solicitará el mensaje:

```text
CIFRAR MENSAJE

Mensaje:
```

Escribe la información que deseas proteger y presiona Enter.

**Paso 4.** Encripta cifrará el mensaje utilizando la clave pública configurada.

**Paso 5.** Al finalizar, mostrará el nombre del archivo generado.

### Ejemplo

Supongamos que deseas enviar a María este mensaje:

"Hola María, la contraseña del documento que acordamos es Primavera2026."

Ejecuta:

```bash
encripta cifrar
```

Ingresa el mensaje:

```text
Mensaje: Hola María, la contraseña del documento que acordamos es Primavera2026.
```

Encripta generará un archivo protegido con extensión `.seg`.

Puedes compartirlo por correo electrónico, WhatsApp u otro medio.

Aunque otra persona tenga acceso al archivo, no podrá leer directamente su contenido. Para recuperarlo necesitará la clave privada correspondiente.

**Importante:** verifica que la clave pública configurada pertenezca al destinatario correcto antes de cifrar.

## 6. Descifrar un mensaje

Esta función permite recuperar el contenido de un mensaje cifrado que otra persona te ha enviado.

### ¿Qué necesitas?

- El archivo cifrado que recibiste.
- Tu clave privada configurada en Encripta.
- La contraseña con la que protegiste tu clave privada.

### Pasos

**Paso 1.** Guarda el archivo cifrado en la ubicación desde la que lo leerá Encripta.

**Paso 2.** Comprueba que tu clave privada esté configurada:

```bash
encripta estado
```

**Paso 3.** Ejecuta el comando de descifrado, indicando el nombre del archivo sin la extensión `.seg`.

Por ejemplo, para descifrar `mensaje.seg`:

```bash
encripta descifrar mensaje
```

También puedes utilizar:

```bash
encripta d mensaje
```

**Paso 4.** Encripta solicitará tu contraseña:

```text
DESCIFRAR MENSAJE

Contraseña:
```

**Paso 5.** Ingresa la contraseña de tu clave privada.

Si los datos son correctos, Encripta mostrará el mensaje original.

### Ejemplo

María te envía un archivo llamado `mensaje.seg`.

Ejecutas:

```bash
encripta descifrar mensaje
```

Ingresas tu contraseña y Encripta recupera el contenido:

```text
El mensaje fue descifrado correctamente.

Mensaje: Hola, te comparto la información confidencial que acordamos.
```

Si utilizas una clave privada diferente o una contraseña incorrecta, no podrás recuperar el contenido.

## 7. ¿Cómo intercambiar mensajes con otra persona?

Imaginemos que Ana y Carlos desean enviarse mensajes confidenciales utilizando Encripta.

### Paso 1. Crear las claves

Ana y Carlos ejecutan en sus respectivos equipos:

```bash
encripta crear-claves
```

Cada uno obtiene su propio par de claves.

### Paso 2. Compartir las claves públicas

Ana envía su clave pública a Carlos y Carlos comparte su clave pública con Ana.

Ninguno debe compartir su clave privada.

### Paso 3. Configurar las claves

Ana configura la clave pública de Carlos y su propia clave privada.

Carlos configura la clave pública de Ana y su propia clave privada.

Ambos utilizan:

```bash
encripta configurar
```

### Paso 4. Enviar un mensaje

Ana ejecuta:

```bash
encripta cifrar
```

Escribe su mensaje y comparte con Carlos el archivo cifrado generado.

### Paso 5. Leer el mensaje

Carlos recibe el archivo, lo coloca en la ubicación correspondiente y ejecuta el comando de descifrado.

Por ejemplo:

```bash
encripta descifrar mensaje
```

Después ingresa la contraseña de su clave privada.

### Paso 6. Responder

Para responder, Carlos ejecuta:

```bash
encripta cifrar
```

Como tiene configurada la clave pública de Ana, podrá generar un mensaje cifrado destinado a ella.

De esta manera, ambos pueden intercambiar mensajes protegidos sin compartir sus claves privadas.

## 8. Recomendaciones de seguridad

Para mantener protegida tu información:

- **Nunca compartas tu clave privada.** Es personal y debe permanecer bajo tu control.
- **No compartas tu contraseña.** Nadie necesita conocerla para enviarte mensajes.
- **Guarda respaldos de tus claves.** Conserva una copia segura de tu clave privada.
- **Verifica las claves públicas.** Asegúrate de que pertenecen a la persona correcta antes de utilizarlas.
- **Protege tu computadora.** Evita que otras personas accedan sin autorización a tus archivos.
- **Conserva tus claves anteriores.** Si generas un nuevo par, podrías necesitar las anteriores para leer mensajes antiguos.
- **Revisa la configuración antes de cifrar.** Confirma que estás utilizando la clave pública del destinatario correcto.

## 9. Preguntas frecuentes

### ¿Necesito conocimientos de programación para utilizar Encripta CLI?

No. Solamente necesitas conocer los comandos básicos y seguir las instrucciones que aparecen en la terminal.

### ¿Necesito compartir mi contraseña para que me envíen mensajes?

No. Solamente necesitas compartir tu clave pública.

### ¿Puedo enviar un mensaje protegido por WhatsApp?

Sí. Puedes compartir el archivo cifrado como documento por WhatsApp, correo electrónico u otro medio.

### ¿Puedo compartir mi clave pública con varias personas?

Sí. Cualquier persona que tenga tu clave pública puede utilizarla para enviarte mensajes cifrados.

### ¿Puedo utilizar una misma clave privada para varios mensajes?

Sí. Puedes utilizarla para recuperar diferentes mensajes que hayan sido cifrados con su clave pública correspondiente.

### ¿Qué sucede si olvido mi contraseña?

No podrás desbloquear tu clave privada protegida sin la contraseña correcta.

### ¿Qué sucede si pierdo mi clave privada?

Si no tienes una copia de respaldo, no podrás recuperar los mensajes cifrados para esa clave.

### ¿Necesito Internet para cifrar o descifrar mensajes?

No. Encripta realiza estas operaciones directamente en tu computadora.

### ¿Qué sucede si cambio de destinatario?

Debes ejecutar nuevamente:

```bash
encripta configurar
```

Luego, indica la clave pública del nuevo destinatario.

### ¿Qué hago si Encripta indica que no hay claves configuradas?

Ejecuta:

```bash
encripta configurar
```

Y registra los nombres de los archivos correspondientes.

### ¿Cómo puedo conocer la versión instalada?

Ejecuta:

```bash
encripta version
```

---

**Encripta — OpenDesarrollo**

[Repositorio oficial](https://github.com/opendesarrollo/Encripta)

*Tu información. Tus decisiones. Tu control.*
