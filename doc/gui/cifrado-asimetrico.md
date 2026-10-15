# Cifrado asimétrico

**Encripta — Manual de usuario (Interfaz gráfica)**

## 1. ¿Qué es el cifrado asimétrico?

El cifrado asimétrico es un método que permite proteger información para que únicamente la persona a quien está destinada pueda leerla.

Para hacerlo, Encripta utiliza dos claves relacionadas entre sí:

- **Clave pública:** puedes compartirla con cualquier persona que desee enviarte mensajes protegidos.
- **Clave privada:** es personal y debes mantenerla en secreto. Se utiliza para recuperar los mensajes que recibes.

Por ejemplo, si deseas enviar un mensaje confidencial a un amigo, necesitas su clave pública para protegerlo. Tu amigo podrá recuperar el mensaje utilizando su clave privada.

**Recuerda:** la clave pública se comparte; la clave privada se protege.

## 2. Crear tus claves

Antes de recibir mensajes cifrados, necesitas generar tus propias claves.

### Pasos

1. Abre la aplicación **Encripta**.
2. En el menú, selecciona **Crear claves**.
3. Ingresa una contraseña.
4. Confirma la contraseña.
5. Haz clic en **Crear claves**.
6. Guarda los dos archivos generados en un lugar seguro.

### ¿Qué archivos obtendrás?

**Clave pública**

Es el archivo que puedes compartir con amigos, familiares o compañeros de trabajo para que puedan enviarte mensajes protegidos.

**Clave privada**

Es el archivo que utilizarás para leer los mensajes cifrados que recibas.

Tu clave privada está protegida mediante la contraseña que estableciste al crearla.

**Importante:** no compartas tu clave privada ni olvides tu contraseña. Si las pierdes, podrías perder el acceso a tus mensajes.

## 3. Configurar tus claves

Encripta permite registrar las claves que utilizarás para enviar y recibir mensajes.

De esta forma, podrás identificarlas fácilmente cuando necesites utilizarlas.

### Agregar una clave pública

1. Ingresa a **Configuración**.
2. Selecciona la opción para agregar una clave pública.
3. Busca el archivo de la clave pública que deseas registrar.
4. Asigna un nombre para identificarla, por ejemplo, `María`.
5. Guarda la clave.

Puedes registrar las claves públicas de diferentes personas.

### Agregar una clave privada

1. Ingresa a **Configuración**.
2. Selecciona la opción para agregar una clave privada.
3. Busca el archivo de tu clave privada.
4. Asigna un nombre para identificarla.
5. Guarda la clave.

Las claves registradas estarán disponibles para seleccionarlas cuando cifres o descifres mensajes.

## 4. Cifrar un mensaje

Esta función permite proteger un mensaje antes de compartirlo con otra persona.

### Pasos

1. En el menú principal, selecciona **Cifrar mensaje**.
2. Escribe el mensaje que deseas proteger.
3. Selecciona la clave pública de la persona que recibirá el mensaje.
4. Haz clic en **Cifrar mensaje**.
5. Una vez completado el proceso, obtén el archivo cifrado generado.

### Ejemplo

Supongamos que deseas enviar a María el siguiente mensaje:

"Hola María, la contraseña del documento que acordamos es Primavera2026."

Al cifrarlo, Encripta genera un archivo protegido con extensión `.seg`.

Puedes enviar este archivo a María por correo electrónico, WhatsApp u otro medio.

Aunque otra persona tenga acceso al archivo, no podrá leer directamente su contenido. Para recuperarlo se necesita la clave privada correspondiente.

**Importante:** asegúrate de seleccionar la clave pública de María antes de cifrar el mensaje.

## 5. Descifrar un mensaje

Esta función permite recuperar el contenido de un mensaje cifrado que otra persona te ha enviado.

### ¿Qué necesitas?

- El archivo cifrado que recibiste.
- Tu clave privada.
- La contraseña con la que protegiste tu clave privada.

### Pasos

1. Abre Encripta.
2. Selecciona **Descifrar mensaje**.
3. Busca y selecciona el archivo `.seg` que recibiste.
4. Selecciona tu clave privada.
5. Ingresa la contraseña correspondiente.
6. Haz clic en **Descifrar mensaje**.

Si la información es correcta, Encripta mostrará el mensaje original.

### Ejemplo

María te envía un archivo llamado `mensaje.seg`.

Al seleccionarlo y descifrarlo con tu clave privada, podrás leer el mensaje que María escribió originalmente.

Si utilizas una clave privada diferente o una contraseña incorrecta, no podrás recuperar el contenido.

## 6. ¿Cómo intercambiar mensajes con otra persona?

Imaginemos que Ana y Carlos desean enviarse mensajes confidenciales utilizando Encripta.

**Paso 1. Crear las claves**

Ana y Carlos generan sus propios pares de claves.

**Paso 2. Compartir las claves públicas**

Ana envía su clave pública a Carlos y Carlos comparte su clave pública con Ana.

Ninguno debe compartir su clave privada.

**Paso 3. Enviar un mensaje**

Ana escribe un mensaje, selecciona la clave pública de Carlos y lo cifra.

Después, envía el archivo generado a Carlos.

**Paso 4. Leer el mensaje**

Carlos abre Encripta, selecciona el archivo recibido, utiliza su clave privada e ingresa su contraseña.

Encripta recupera el mensaje original.

**Paso 5. Responder**

Si Carlos desea responder de forma protegida, utiliza la clave pública de Ana para cifrar su respuesta.

De esta manera, ambos pueden intercambiar mensajes protegidos sin compartir sus claves privadas.

## 7. Recomendaciones de seguridad

Para mantener protegida tu información:

- **Nunca compartas tu clave privada.** Es personal y debe permanecer bajo tu control.
- **No compartas tu contraseña.** Nadie necesita conocerla para enviarte mensajes.
- **Guarda respaldos de tus claves.** Conserva una copia de tu clave privada en un lugar seguro.
- **Verifica las claves públicas.** Asegúrate de que pertenecen a la persona correcta antes de utilizarlas.
- **Protege tu computadora.** Evita que otras personas accedan sin autorización a tus archivos.
- **Conserva tus claves anteriores.** Si generas un nuevo par, podrías necesitar las anteriores para leer mensajes antiguos.

## 8. Preguntas frecuentes

### ¿Necesito compartir mi contraseña para que me envíen mensajes?

No. Solamente necesitas compartir tu clave pública.

### ¿Puedo enviar un mensaje protegido por WhatsApp?

Sí. Puedes enviar el archivo cifrado como documento por WhatsApp, correo electrónico u otro medio.

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

### ¿Qué sucede si envío el archivo a la persona equivocada?

El contenido permanecerá cifrado. Sin embargo, cualquier persona que tenga acceso a la clave privada correspondiente y pueda desbloquearla podría recuperarlo.

---

**Encripta — OpenDesarrollo**

[Repositorio oficial](https://github.com/opendesarrollo/Encripta)

*Tu información. Tus decisiones. Tu control.*
