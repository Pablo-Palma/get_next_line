
# Get Next Line


📖 **Bienvenido a Get Next Line (GNL)**

**Get Next Line** es una implementación en C para la gestión de lecturas, optimizada para recuperar líneas desde un archivo o descriptor de archivo. Su diseño garantiza precisión en operaciones de lectura, facilitando la manipulación detallada de archivos.


🌟 **Características Principales**

- **Tamaño de Buffer Personalizable:** Compila con el flag `-D BUFFER_SIZE=xx` para determinar el tamaño del buffer para las lecturas. Ejemplo con un tamaño de buffer de 42: `cc -Wall -Werror -Wextra -D BUFFER_SIZE=42 <archivos>.c`.

- **Lectura Eficiente:** GNL lee el archivo en fragmentos, en lugar de cargar todo en memoria. Si detecta un salto de línea, devuelve inmediatamente esa línea sin procesar el archivo completo.

- **Compatibilidad Amplia:** Prueba GNL con diversos tamaños de BUFFER_SIZE, desde 1 hasta 10000000, para garantizar una operación óptima en cualquier escenario.

🔐 **Consideraciones**

- **Cambios en el Archivo:** Si el archivo apuntado por el fd cambia desde la última llamada (y no se ha llegado al final del archivo mediante `read()`), el comportamiento de GNL es indeterminado.

📋 **Directrices de Compilación**

- Puedes compilar con o sin el flag `-D BUFFER_SIZE`, según lo necesites. El valor por defecto es flexible según tus preferencias.


---

¿Tienes inquietudes o sugerencias? Contacta al desarrollador.

📞 **Contacto**

- **GitHub:** [Pablo-Palma](https://github.com/Pablo-Palma)
  
- **Email:** pablopalmappr@gmail.com

---
