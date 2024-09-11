# project_part4

docker tag book-catalog sit722cnpart4.azurecr.io/book-catalog:latest

docker tag inventory-management sit722cnpart4.azurecr.io/inventory-management:latest

docker login sit722cnpart4.azurecr.io

docker push sit722cnpart4.azurecr.io/book-catalog:latest

docker push sit722cnpart4.azurecr.io/inventory-management:latest

az acr repository list --name sit722cnpart4 --output table

az aks get-credentials --resource-group sit722cnpart4 --name sit722cnpart4 --overwrite-existing
