## Instalacion

1. Con la terminal en la ubicación deseada, clonar este repo y su dependencia:
   ```
   git clone git@bitbucket.org:radaresfacet/simulador_core.git@dev
   git clone git@bitbucket.org:radaresfacet/dependencias_estaticas.git
   ```

2. Crear un nuevo ambiente. Se muestran las instrucciones para crear uno usando la herramienta venv:
    Para Windows:
    ```   
    cd simulador_core
    python -m venv .venv
    .venv\Scripts\activate
    python -m pip install -U pip
    ``` 

3. Para instalar las dependencias de este proyecto, desde el ambiente ejecutar:
    ```
    pip install -U -r yolov5/requirements.txt
    pip install -U -r XmlToTxt/requirements.txt
    ```