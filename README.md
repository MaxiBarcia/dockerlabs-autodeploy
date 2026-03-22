#  DockerLabs AutoDeploy

Script automatizado para desplegar máquinas vulnerables de DockerLabs con mapeo inteligente de puertos y gestión de logs.

##  Características

-  **Despliegue automático** de cualquier máquina DockerLabs en formato `.tar`
-  **Mapeo inteligente de puertos** - Detecta y evita conflictos
-  **Logs persistentes** - Guarda los logs en `/home/cft/logs_victima`
-  **Limpieza automática** - Elimina contenedores e imágenes al presionar Ctrl+C
-  **Interfaz colorida** - Información clara y fácil de entender
-  **Gestión de conflictos** - Detecta puertos ocupados y busca alternativas

##  Requisitos

- Linux (probado en Kali Linux)
- Docker instalado (el script lo instala automáticamente si no está presente)
- Permisos de sudo (para instalación de Docker)

##  Instalación

```bash
# Clonar el repositorio
git clone https://github.com/MaxiBarcia/dockerlabs-autodeploy.git
cd dockerlabs-autodeploy

# Dar permisos de ejecución
chmod +x auto_deploy.sh

# Opcional: mover a /usr/local/bin para usarlo desde cualquier lugar
sudo cp auto_deploy.sh /usr/local/bin/dockerlab
