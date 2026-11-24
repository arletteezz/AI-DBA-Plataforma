# AI-DBA Plataforma

Aplicación web diseñada para brindar una interfaz intuitiva y segura para la administración, monitoreo, optimización, respaldo y gestión de seguridad de instancias de Microsoft SQL Server.

## Tecnologías Utilizadas
* **Backend:** Python, FastAPI, Uvicorn, SQLAlchemy.
* **Base de Datos:** Microsoft SQL Server (`dba_plataforma`).
* **Seguridad:** Cifrado de contraseñas con bcrypt (PBKDF2-HMAC-SHA256) y autenticación mediante tokens JWT.
* **Frontend:** HTML5 y CSS3.

## Estructura del Proyecto
* `main.py` - Código principal del servidor
* `servidor.py` - Script de arranque
* `src/conexion/conexion_bd.py` - Conexión a SQL Server
* `src/modelos.py` - Modelos de la base de datos
* `src/seguridad.py` - Contraseñas y tokens JWT
* `src/crud.py` - Operaciones de base de datos
* `templates/` - Páginas HTML (base, login, inicio, instancias, monitoreo, optimizacion, respaldo, seguridad)
* `static/` - Archivos CSS e imágenes
* `venv/` - Entorno virtual de Python

## Requisitos Previos
* Python instalado.
* Microsoft SQL Server (con la base de datos `dba_plataforma` creada).
* Git.

## Instalación y Ejecución
1. **Clonar el repositorio:**
   `git clone https://github.com/arletteezz/AI-DBA-Plataforma.git`
   `cd AI-DBA-Plataforma`

2. **Activar el entorno virtual (Windows PowerShell):**
   `Set-ExecutionPolicy -Scope Process RemoteSigned`
   `.\venv\Scripts\Activate.ps1`

3. **Instalar dependencias:**
   `pip install fastapi uvicorn sqlalchemy pyodbc passlib[bcrypt] python-jose`

4. **Iniciar el servidor:**
   `venv\Scripts\python.exe servidor.py`

5. **Acceder al sistema:**
   * Interfaz Web: http://127.0.0.1:8000
   * Documentación de la API (Swagger): http://127.0.0.1:8000/docs

## Credenciales de Prueba
* **Usuario:** `dilanZMEX`
* **Contraseña:** `20050929`
* **Rol:** Administrador
