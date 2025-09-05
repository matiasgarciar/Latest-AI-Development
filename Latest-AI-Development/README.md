# Latest AI Development – Sección 2.2.1 del TFG

Este repositorio contiene el código de la **sección 2.2.1 “Componentes internos del Agente”** del Trabajo de Fin de Grado *Exploración de sistemas multi-agente en IA generativa*.  

El material corresponde al ejemplo utilizado para ilustrar la **Figura 2.2** de la memoria, donde se muestran los elementos principales que componen un agente dentro de un sistema multi-agente.

---

##  Estructura del repositorio

- `Latest-AI-Development/src/latest_ai_development/` → Código fuente principal del agente  
  - `main.py` → Punto de entrada  
  - `crew.py` → Definición de la orquestación de agentes  
  - `tools/` → Herramientas personalizadas utilizadas por el agente  
  - `config/` → Ficheros YAML con la configuración de agentes y tareas  
- `requirements.txt` → Dependencias mínimas (instalables con `pip`)  
- `.env.example` → Plantilla de credenciales (copiar a `.env` y completar con las claves reales)  
- `.gitignore` → Exclusiones recomendadas (evita subir `.env`, `.venv`, cachés, etc.)  

---

##  Instalación y ejecución

```bash
# Clonar el repositorio
git clone https://github.com/matiasgarciar/Latest-AI-Development.git
cd Latest-AI-Development

# Crear un entorno virtual (opcional pero recomendado)
python -m venv .venv
source .venv/bin/activate   # en Linux/Mac
.venv\Scripts\activate      # en Windows

# Instalar dependencias
pip install -r requirements.txt

# Configurar variables de entorno
cp .env.example .env   # y añadir las claves necesarias (ej. OPENAI_API_KEY)

# Ejecutar el agente
python Latest-AI-Development/src/latest_ai_development/main.py


