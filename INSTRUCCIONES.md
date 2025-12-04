# 🧟 Instrucciones para Ejecutar la Operación Anti-Zombie

## Configuración del Entorno Virtual

### 1. Activar el entorno virtual

**En Windows PowerShell:**
```powershell
.\venv\Scripts\Activate.ps1
```

**En Windows CMD:**
```cmd
venv\Scripts\activate.bat
```

**En Linux/Mac:**
```bash
source venv/bin/activate
```

### 2. Verificar que el entorno está activo

Deberías ver `(venv)` al inicio de tu línea de comandos.

### 3. Instalar dependencias (si aún no están instaladas)

```bash
pip install -r requirements.txt
```

## Ejecutar el Notebook

### Opción 1: Jupyter Notebook

```bash
jupyter notebook operacion_anti_zombie.ipynb
```

### Opción 2: Jupyter Lab

```bash
jupyter lab operacion_anti_zombie.ipynb
```

### Opción 3: VS Code

Abre el archivo `operacion_anti_zombie.ipynb` directamente en VS Code y selecciona el kernel de Python del entorno virtual.

## Estructura del Proyecto

```
EV3_IDN/
├── data/
│   ├── evolucion_brote.xlsx
│   ├── pacientes_brote_zombie.xlsx
│   ├── red_contagios.xlsx
│   └── tratamientos_experimentales.xlsx
├── venv/                    # Entorno virtual (no versionar)
├── operacion_anti_zombie.ipynb
├── requirements.txt
└── INSTRUCCIONES.md
```

## Notas Importantes

- Asegúrate de que el entorno virtual esté activado antes de ejecutar el notebook
- Los datos deben estar en la carpeta `data/` con los nombres exactos indicados
- El notebook está estructurado siguiendo las 5 misiones de la Operación Anti-Zombie
- Ejecuta las celdas en orden para obtener los resultados completos

## Solución de Problemas

### Error al activar el entorno virtual en PowerShell

Si obtienes un error de política de ejecución, ejecuta:
```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### Error al importar librerías

Asegúrate de que el entorno virtual esté activado y que todas las dependencias estén instaladas:
```bash
pip install -r requirements.txt
```

