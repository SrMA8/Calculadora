# 🔐 Calculadora CHMOD

Aplicación web interactiva que permite comprender y calcular los permisos de archivos en Linux utilizando la notación numérica (octal) del comando `chmod`.

La herramienta permite seleccionar permisos de forma visual o introducir directamente el número octal, generando automáticamente el comando correspondiente en tiempo real.

---

## ✨ Características

* Cálculo de permisos CHMOD en tiempo real
* Conversión bidireccional:

  * Selección visual → Número octal
  * Número octal → Permisos visuales
* Generación automática del comando `chmod`
* Validación de entrada (solo valores del **0 al 7**)
* Interfaz limpia, moderna y centrada
* Proyecto sin dependencias externas (JavaScript puro)

---

## 🧠 Lógica de permisos en Linux

Cada permiso tiene un valor numérico:

| Permiso  | Valor |
| -------- | ----- |
| Leer     | 4     |
| Escribir | 2     |
| Ejecutar | 1     |

Los permisos se agrupan en:

* **Usuario**
* **Grupo**
* **Otros**

Ejemplo:

```bash id="w0k0ap"
Usuario: Lectura + Escritura + Ejecución = 7  
Grupo: Lectura + Ejecución = 5  
Otros: Lectura + Ejecución = 5  

chmod 755 archivo.txt
```

---

## 🏗️ Estructura del proyecto

```id="l03nr0"
calculadora-chmod/
│
├── index.html
├── style.css
└── README.md
```

---

## 🚀 Cómo ejecutar el proyecto

### 1. Clonar el repositorio

```bash id="mra5er"
git clone https://github.com/tuusuario/calculadora-chmod.git
```

### 2. Abrir el proyecto

Simplemente abre el archivo:

```id="9hbf12"
index.html
```

en cualquier navegador web.

No requiere instalación ni herramientas adicionales.

---

## 🎮 Uso

### Modo visual

1. Selecciona los permisos para:

   * Usuario
   * Grupo
   * Otros
2. El número CHMOD se actualizará automáticamente
3. El comando de terminal se generará en tiempo real

### Modo numérico

1. Introduce un número octal de 3 dígitos (ej. `644`, `755`, `700`)
2. La interfaz marcará automáticamente los permisos correspondientes

---

## 🎯 Objetivo del proyecto

Este proyecto fue desarrollado como práctica para:

* Comprender el sistema de permisos en Linux
* Practicar manipulación del **DOM con JavaScript**
* Construir una interfaz interactiva usando **HTML y CSS puro**
* Fortalecer fundamentos de desarrollo Frontend sin frameworks

---

## 🔮 Posibles mejoras

* Soporte para notación simbólica (`rwxr-xr-x`)
* Botón para copiar el comando
* Campo editable para el nombre del archivo
* Modo oscuro / claro
* Optimización móvil
* Publicación con GitHub Pages

---

## 👨‍💻 Autor

Proyecto desarrollado con fines educativos y de práctica en desarrollo web.

---

## 📄 Licencia

MIT — libre uso, modificación y distribución.
