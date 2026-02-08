# Netology_K8S_1.4 (Моисеенко А.Н.) 

## Задание 1: Настройка Service (ClusterIP и NodePort)

### Развернуть приложение из двух контейнеров (nginx и multitool) и обеспечить доступ к ним:

- Внутри кластера через ClusterIP.
- Снаружи через NodePort.
  
### Скриншоты проверки доступа (curl или браузер):

- curl web-service:9001
<img width="1164" height="475" alt="image" src="https://github.com/user-attachments/assets/56d39b4e-4e84-42cc-93c4-c397ed6c517d" />

- curl web-service:9001
<img width="1050" height="58" alt="image" src="https://github.com/user-attachments/assets/cf5c5119-24be-457d-85b0-2d4dc60e6bd4" />

- curl http://172.16.20.43:30080
<img width="1105" height="465" alt="image" src="https://github.com/user-attachments/assets/fe9e46bd-329f-4416-95d1-a5d2e56dfbcd" />
### Манифесты:

- [deployment-multi-container.yaml]()
- [service-clusterip.yaml]()
- [service-nodeport.yaml]()


