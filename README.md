# Sistema-de-registro-de-usuarios
# Sistema de Registro de Usuarios

## Descripción del Caso
Este proyecto consiste en el desarrollo de un sistema básico de registro de usuarios que permita almacenar, validar y gestionar la información personal de nuevos usuarios. El sistema está diseñado para entornos académicos o aplicativos web donde se requiere administrar cuentas de acceso de forma segura y ordenada. Su principal objetivo es garantizar que cada usuario pueda crear una cuenta única mediante un proceso sencillo, eficiente y confiable.

---

## Objetivos del Sistema
1. Permitir el registro de nuevos usuarios mediante un formulario con validación de datos.
2. Garantizar la unicidad del usuario, evitando duplicidad mediante verificación de correo o nombre de usuario.
3. Almacenar la información de forma segura respetando principios de confidencialidad e integridad.
4. Proveer retroalimentación clara al usuario en caso de errores o datos incompletos.
5. Ofrecer una base para futuros módulos como inicio de sesión, recuperación de contraseña o gestión de perfiles.

---

## Requerimientos del Sistema

### Requerimientos Funcionales
1. **RF1:** El sistema debe permitir ingresar datos personales: nombre, correo y contraseña.
2. **RF2:** El sistema debe validar que el correo electrónico no esté registrado previamente.
3. **RF3:** El sistema debe encriptar la contraseña antes de almacenarla.
4. **RF4:** El sistema debe notificar al usuario si el registro fue exitoso o si hubo errores.
5. **RF5:** El sistema debe almacenar los datos del usuario en una base de datos o archivo persistente.

### Requerimientos No Funcionales
1. **RNF1:** El sistema debe responder en menos de 2 segundos durante el proceso de registro.
2. **RNF2:** La interfaz debe ser intuitiva y fácil de usar.
3. **RNF3:** La información debe almacenarse cumpliendo criterios de seguridad y privacidad.

---

## Tabla de Pruebas

| Caso de Prueba | Entrada | Proceso | Resultado Esperado | Estado |
|----------------|---------|---------|--------------------|--------|
| CP01 | Datos completos y válidos | Validación y registro | Usuario registrado con éxito | Aprobado |
| CP02 | Correo ya registrado | Verificar duplicidad | Mensaje de error: “correo ya existe” | Aprobado |
| CP03 | Contraseña vacía | Validar campos | Mensaje de error | Aprobado |
| CP04 | Formato de correo incorrecto | Verificar formato | Solicitar corrección | Aprobado |
| CP05 | Desconexión de base de datos | Intentar registrar | Notificar falla del servidor | Aprobado |

---

## Tipo de Mantenimiento Propuesto

### Mantenimiento Correctivo
Solucionar errores relacionados con validación, fallos en la base de datos o registros incompletos.

### Mantenimiento Perfectivo
Mejorar la experiencia del usuario, agregar validaciones más robustas o ampliar campos del formulario.

### Mantenimiento Evolutivo
Integrar funciones adicionales como inicio de sesión, roles de usuario, recuperación de contraseña o autenticación mediante redes sociales.

---

## Reflexión Final
El sistema de registro de usuarios constituye un elemento fundamental en prácticamente cualquier plataforma moderna. Su correcta implementación garantiza seguridad, usabilidad y confianza por parte de los usuarios. Además, actúa como punto de partida para funcionalidades más avanzadas, por lo que debe construirse con buenas prácticas y criterios escalables. Un sistema sencillo pero bien estructurado puede crecer de manera orgánica e integrarse con módulos que requieren autenticación y personalización, convirtiéndose en un pilar dentro del desarrollo de software.
