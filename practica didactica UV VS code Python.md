Perfecto. Aquí tienes una **práctica didáctica estructurada** para implementar **UV + Python + VS Code**, lista para usar en clase, con enfoque progresivo y operativo.

---

# 🧪 PRÁCTICA: Proyecto Python con UV

## 🎯 Objetivo

Que el alumno:

* Configure un entorno moderno con **uv**
* Cree un proyecto Python estructurado
* Instale dependencias
* Ejecute código correctamente

---

## 🧰 Herramientas requeridas

* **Python** (>= 3.10)
* **Visual Studio Code**
* Terminal (PowerShell o CMD)
* **UV instalado**

---

# 🟢 FASE 1: Preparación del entorno

### 1. Verificar Python

```bash
python --version
```

---

### 2. Verificar UV

```bash
uv --version
```

---

### 3. Abrir VS Code

* Crear carpeta:

```bash
crud_uv
```

* Abrir en VS Code:

```bash
code crud_uv
```

---

# 🟡 FASE 2: Inicializar proyecto con UV

Dentro de la carpeta:

```bash
uv init
```

Esto generará archivos base del proyecto.

---

# 📁 Estructura inicial generada

```plaintext
crud_uv/
│
├── pyproject.toml        # Configuración del proyecto
├── README.md             # Descripción
├── .python-version       # Versión de Python
└── main.py               # Archivo principal
```

---

# 🔵 FASE 3: Organización profesional del proyecto

Modificar estructura a:

```plaintext
crud_uv/
│
├── app/                  # Lógica principal
│   ├── __init__.py
│   ├── main.py
│   ├── models.py
│   ├── services.py
│   └── utils.py
│
├── data/                 # Datos o base de datos
│   └── database.db
│
├── tests/                # Pruebas
│   └── test_main.py
│
├── .venv/                # Entorno virtual (automático con UV)
├── pyproject.toml
├── README.md
└── .python-version
```

---

# 🟠 FASE 4: Crear archivos base

### 📌 app/main.py

```python
def main():
    print("Proyecto Python con UV funcionando")

if __name__ == "__main__":
    main()
```

---

### 📌 app/models.py

```python
class Empleado:
    def __init__(self, nombre, puesto):
        self.nombre = nombre
        self.puesto = puesto
```

---

### 📌 app/services.py

```python
def crear_empleado(nombre, puesto):
    return {"nombre": nombre, "puesto": puesto}
```

---

### 📌 app/utils.py

```python
def imprimir_mensaje(msg):
    print(f"[INFO]: {msg}")
```

---

# 🟣 FASE 5: Instalar dependencias con UV

Ejemplo:

```bash
uv add requests
```

Esto actualiza automáticamente:

```toml
# pyproject.toml
dependencies = [
    "requests"
]
```

---

# 🔴 FASE 6: Ejecutar el proyecto

Desde la raíz:

```bash
uv run app/main.py
```

---

# ⚙️ FASE 7: Configuración en VS Code

### Extensiones recomendadas:

* Python
* Pylance

---

### Seleccionar intérprete:

1. Ctrl + Shift + P
2. "Python: Select Interpreter"
3. Elegir `.venv`

---

# 🧪 FASE 8: Actividad práctica para alumnos

## 📝 Ejercicio

Desarrollar un mini CRUD:

* Crear empleado
* Listar empleados
* Buscar empleado

---

## 📌 Ejemplo simple en main.py

```python
empleados = []

def agregar():
    nombre = input("Nombre: ")
    puesto = input("Puesto: ")
    empleados.append({"nombre": nombre, "puesto": puesto})

def listar():
    for e in empleados:
        print(e)

def menu():
    while True:
        print("\n1. Agregar\n2. Listar\n3. Salir")
        op = input("Opción: ")

        if op == "1":
            agregar()
        elif op == "2":
            listar()
        elif op == "3":
            break

if __name__ == "__main__":
    menu()
```

---

# 🧩 FASE 9: Evaluación

### Criterios:

| Criterio                | Puntos |
| ----------------------- | ------ |
| Instalación correcta    | 20     |
| Estructura del proyecto | 20     |
| Uso de UV               | 20     |
| Código funcional        | 20     |
| Organización            | 20     |

---

# 🎯 Cierre pedagógico

El alumno comprende:

* Gestión moderna de proyectos Python con **UV**
* Separación de responsabilidades (estructura tipo profesional)
* Ejecución controlada de código
* Preparación para frameworks más avanzados

---

## 🚀 Siguiente paso sugerido

Puedo convertir esto en:

* ✔️ Proyecto completo CRUD con SQLite
* ✔️ Integración con Firebase (como ya trabajas)
* ✔️ Versión con interfaz gráfica o API

Solo dime el nivel (básico, intermedio o avanzado) y lo estructuro.
