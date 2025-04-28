
# Setup AKS Cluster & Deploy Springboot Docker Container to AKS Cluster using Helm and Azure Pipeline

First I have created simple Spring Boot Java project in Intellij

![alt text](image.png)

Compiled using Maven and jar got generated in target folder

![alt text](image-1.png)

Running the app locally before pushing to AKS

Application running and getting  the result. Port is exposed to 8080

![alt text](image-2.png)

Next step. Will use Azure CLI to connect to Azure portal

 az login
 
 ![alt text](image-3.png)

 Selected my subscription 

 Next step is to create AKS cluster to deploy Java App. I have created script to handle that
 ![alt text](image-4.png)

It started creating resources defined in script file

![alt text](image-5.png)

All resources are created

![alt text](image-7.png)

Cluster is running

![alt text](image-8.png)

![alt text](image-9.png)

creating helm chart using create helm chart command  helm create my-aks-chart

![alt text](image-11.png)
Helm chart is created with all yaml templates


![alt text](image-12.png)

Create pipeline and choose classic editor

![alt text](image-13.png)

![alt text](image-14.png)