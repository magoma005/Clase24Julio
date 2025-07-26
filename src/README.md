# 🐾 Clase24Julio - Gestión de Mascotas

Este proyecto en Java implementa una aplicación de escritorio con interfaz gráfica (Swing) para gestionar un registro de mascotas, utilizando serialización para la persistencia de datos. Incluye una arquitectura organizada en capas DAO, DTO, vista y persistencia, siguiendo buenas prácticas de programación.

---

## 📦 Estructura del Proyecto

Clase24Julio/
│
├── data/ # Archivos serializados (salvado de datos)
├── out/ # Archivos compilados
├── src/
│ ├── dao/ # Lógica de acceso a datos
│ │ └── MascotaDAO.java
│ ├── dto/ # Modelo de datos
│ │ └── MascotaDTO.java
│ ├── excepciones/ # Excepciones personalizadas
│ │ └── DatoInvalidoException.java
│ ├── persistencia/ # Gestor de serialización
│ │ └── GestorPersistencia.java
│ ├── vista/ # Interfaz gráfica (Swing)
│ │ └── FormMascota.java
│ └── Main.java # Clase principal
│
├── .gitignore
└── Clase24Julio.iml

---

## ✨ Funcionalidades

- Registrar mascotas con nombre, especie y edad.
- Listar todas las mascotas guardadas.
- Editar los datos de una mascota seleccionada.
- Eliminar mascotas del registro.
- Validación de entradas (datos obligatorios y edad numérica).
- Persistencia local usando serialización (`.dat`).

---

## 💻 Tecnologías usadas

- **Java SE**
- **Swing** para GUI
- **Persistencia**: serialización con `ObjectOutputStream` y `ObjectInputStream`
- **Arquitectura MVC ligera**

---

## 🚀 Cómo ejecutar

1. Asegúrate de tener **JDK 8 o superior** instalado.
2. Clona este repositorio o descarga el código fuente.
3. Abre el proyecto en **IntelliJ IDEA** o **NetBeans**.
4. Ejecuta la clase `Main.java`.
5. ¡Listo! Se abrirá una ventana para registrar y gestionar mascotas.

---

## 📁 Persistencia de datos

Los datos se almacenan automáticamente en `data/mascotas.dat`. Esta carpeta se crea en la raíz del proyecto si no existe.

---

## 🔒 Validaciones

El formulario valida que:
- Todos los campos estén completos.
- La edad sea un número entero no negativo.

Los errores se muestran mediante cuadros de diálogo.

---

## 🧠 Autor

**Miguel Ángel Guarín**  
Desarrollador de software en formación.  
Apasionado por Java, Swing y buenas prácticas de programación.

---

## 📃 Licencia

Este proyecto es de uso educativo y no tiene licencia comercial.