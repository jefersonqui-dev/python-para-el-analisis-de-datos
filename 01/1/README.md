# 01 - Fundamentos modernos para el analisis de datos con python

## Clase 1 - Configuracion Profesional del Entorno y Primer Proyecto

### 1. Configuracion del Entorno de Desarrollo Profesional

#### 1.1 Instalación de Python
- **Descargar Python**: Visitar [python.org](https://python.org) y descargar la versión más reciente (3.11+)
- **Instalación**: Ejecutar el instalador marcando "Add Python to PATH"
- **Verificar**: Abrir terminal y ejecutar `python --version`

#### 1.2 Configuración del Entorno Virtual
```bash
# Crear entorno virtual
python -m venv mi_proyecto

# Activar entorno virtual
# Windows:
mi_proyecto\Scripts\activate
# macOS/Linux:
source mi_proyecto/bin/activate

# Desactivar
deactivate
```

#### 1.3 Gestión de Paquetes
```bash
# Actualizar pip
python -m pip install --upgrade pip

# Instalar paquetes
pip install nombre_paquete

# Instalar desde requirements.txt
pip install -r requirements.txt

# Generar requirements.txt
pip freeze > requirements.txt
```

#### 1.4 Herramientas Esenciales
```bash
# Jupyter Notebook (para análisis de datos)
pip install jupyter

# Pandas (manipulación de datos)
pip install pandas

# NumPy (computación numérica)
pip install numpy

# Matplotlib (visualización)
pip install matplotlib

# Seaborn (visualización estadística)
pip install seaborn
```

#### 1.5 Configuración del IDE
- **VS Code**: Instalar extensión "Python" de Microsoft
- **PyCharm**: Configurar intérprete Python del entorno virtual
- **Spyder**: Incluido con Anaconda

#### 1.6 Estructura de Proyecto Recomendada
```
mi_proyecto/
├── src/
│   ├── __init__.py
│   └── main.py
├── data/
├── notebooks/
├── tests/
├── requirements.txt
├── README.md
└── .gitignore
```

#### 1.7 Comandos Útiles
```bash
# Ejecutar script Python
python script.py

# Ejecutar con argumentos
python script.py arg1 arg2

# Modo interactivo
python

# Ejecutar tests
python -m pytest

# Linting y formateo
pip install flake8 black
flake8 src/
black src/
```

#### 1.8 Configuración de Git (Opcional)
```bash
# Inicializar repositorio
git init

# Crear .gitignore
echo "venv/" > .gitignore
echo "__pycache__/" >> .gitignore
echo "*.pyc" >> .gitignore
echo ".ipynb_checkpoints/" >> .gitignore
```

### 2. Verificación de la Configuración
```python
# Crear archivo test_config.py
import sys
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

print(f"Python version: {sys.version}")
print(f"Pandas version: {pd.__version__}")
print(f"NumPy version: {np.__version__}")
print("¡Configuración exitosa!")
```

### 3. Próximos Pasos
- Crear primer proyecto con Jupyter Notebook
- Explorar funcionalidades básicas de Pandas
- Practicar con datasets de ejemplo
