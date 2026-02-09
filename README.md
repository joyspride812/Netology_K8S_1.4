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

## Задание 2: Развернуть два приложения (frontend и backend) и обеспечить доступ к ним через Ingress по разным путям.

### Результат запроса curl http://testapp.local/
<img width="755" height="415" alt="image" src="https://github.com/user-attachments/assets/c553a6b1-58f2-48e3-928d-b40d53fb4bc6" />


### Результат запроса curl http://testapp.local/api
<img width="1185" height="131" alt="image" src="https://github.com/user-attachments/assets/970c5dc0-84c7-484c-b0ea-9b26bddcd3d2" />

### Манифесты:
- [backend.yaml](https://github.com/joyspride812/Netology_K8S_1.4/blob/main/backend.yaml)
- [frontend.yaml](https://github.com/joyspride812/Netology_K8S_1.4/blob/main/frontend.yaml)
- [service-backend.yaml](https://github.com/joyspride812/Netology_K8S_1.4/blob/main/service-backend.yaml)
- [service-frontend.yaml](https://github.com/joyspride812/Netology_K8S_1.4/blob/main/service-frontend.yaml)
- [ingress.yaml](https://github.com/joyspride812/Netology_K8S_1.4/blob/main/ingress.yaml)





