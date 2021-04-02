# triviawebapp-platzicurso
platzicurso-gce
# Practicas
¿Qué es compute engine?
El servicio de Google
Cloud Platform (GCP)
para crear VM.
.- VM Personalizables y estandarizadas.
.- De proposito general
.- compatibles con Linux y Windows
.- VM efimeras y permanentes

.-Crear un VM con metadata:
gcloud compute instansce create vm-ejemplo --metadata clave=valor
.-Agregar metadata a una VM existente:
gcloud compute instances add-metadata vm-ejemplo --metadata tortilla=doble

● Creación de vm con metadata
gcloud compute instances create vm-ejemplo \
--scopes storage-ro \
--metadata \
startup-script-url=gs://bucket/startupscript.sh

● Un startup script puede lucir así
#/bin/bash
sudo apt update
sudo apt install apache2 -y

.-Creación de vm con shutdown script 
gcloud compute instances create your-instance \ --metadata-fron-file \ shutdown-script-examples/scripts/install.sh
project name :  curso-gce-platzi
 Project ID: curso-gce-platzi-30942

 https://console.cloud.google.com/home/dashboard?project=curso-gce-platzi-309423&organizationId=0
