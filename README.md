# Google Cloud Platform

Deploy Golang Application on Google Cloud Run

# Requisitos:
 - Tener una cuenta en GCP activa.
 - Tener un proyecto creado en GCP <PROJECT-ID>.
 - Tener habilitada la facturación para tu proyecto de GCP.
 - Tener habilitadas las Cloud Build and Cloud Run API.
 
 
# Pasos:

1.- Instalar el SDK de Cloud.
- $ /usr/local/Cellar/google-cloud-sdk/install.sh

2.- Actualización de componentes
- $ gcloud components update

3.- Crear proyecto Golang

4.- Crear archivo Dockerfile

5.- Construir imagen
- $ gcloud builds submit --tag gcr.io/<PROJECT-ID>/helloworld

6.- Desplegar imagen en Cloud Run
- $ gcloud run deploy --image gcr.io/playgroundtwchile/helloworld --platform managed --allow-unauthenticated

7.- Verifcar funcionalidad 
- https://helloworld-a7kkp73naa-uc.a.run.app


