# test_kubernetes
У нас должен быть кластер Kubernetes, а инструмент командной строки kubectl должен быть настроен для связи с вашим кластером.

Затем вводим следующие 4 команды для запуска микросервиса:

1) kubectl apply -f backend-deployment.yaml
(kubectl describe deployment backend - посмотреть инфу о backend deployment)

2) kubectl apply -f backend-service.yaml

3) kubectl apply -f frontend-deployment.yaml

4) kubectl apply -f frontend-service.yaml

После того, как создали сервис, можем использовать команду 
 kubectl get service frontend --watch для поиска внешнего IP-адреса

Нужно взять значение столбца EXTERNAL-IP и проверить запрос
