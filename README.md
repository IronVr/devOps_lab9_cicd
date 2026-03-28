# devOps_lab9_cicd
## Цель работы
Создаем Cloud-native приложение для экспериментов, реализовать:
- Создаем приложение;
- Создаем uint-tests для приложения;
- Докеризируем: Создаем докерфайл для сборки контейнера;
- Описываем CI-сценарии для Github Actions производящие lint, unit-test, build-test;
- Куберизируем: Создаем манифесты для запуска приложения и сервисов в кластере;
- Описываем CD-сценарии для Github Actions производящие docker build и push в Docker Hub;
- Устанавливаем ArgoCD и подключаем к GitHub;
- Проверяем весь CI/CD workflow в сборе;
## Методические указания
  * Для выполнения работы необходимы знания, полученные при выполнении прошлых;
  * План выполнения работ находится тут: [2026_DevOps__Л11_П11_CICD.pdf](https://github.com/user-attachments/files/26323085/2026_DevOps__.11_.11_CICD.pdf).

## Проверка результатов
  * Проверяем CI-сценарии
<img width="1852" height="797" alt="проверка работы сценария CI" src="https://github.com/user-attachments/assets/24193320-c662-4d28-8896-e9dae44f4148" />
<img width="830" height="328" alt="lint и unit tests ок" src="https://github.com/user-attachments/assets/a6245ddd-48b5-41b6-a9a8-b9c9aa368394" />

  * Проверяем работу сервера
<img width="482" height="357" alt="получили доступ" src="https://github.com/user-attachments/assets/bcde2dd6-a2ee-4429-b727-723e22dad79c" />

  * Добавляем свои учетные данные как Action Secrets на Github
<img width="992" height="242" alt="секреты" src="https://github.com/user-attachments/assets/7b3452df-256b-43f2-912c-417060ede007" />

  * Проверяем работу pipeline
<img width="1246" height="425" alt="успешный пайп" src="https://github.com/user-attachments/assets/11112d25-75c5-42f4-890d-57be1d640314" />

  * Pipeline успешно положил образ в DockerHub
<img width="898" height="706" alt="положили образ в докер заб" src="https://github.com/user-attachments/assets/26cf0d5c-cabf-42c7-8afd-172957cde0bd" />

  * Запускаем ArgoCD
<img width="1477" height="737" alt="успешно зашли в argo cd" src="https://github.com/user-attachments/assets/a119c6de-1599-4a63-97c5-0695f53d986d" />

  * Подключаем репозиторий к ArgoCD
<img width="1350" height="207" alt="подключили репо к арго" src="https://github.com/user-attachments/assets/2e7dfaf5-dc7e-4c90-8ef3-4558451f1bd9" />

  * Подключаем манифесты и проверяем работу
<img width="1611" height="632" alt="argo все четко" src="https://github.com/user-attachments/assets/860d58be-ecb2-4725-bda3-2de3c4d2385a" />

  * После правок в dockerfile и index.html создаем MR и проверяем работу тестов
<img width="1125" height="560" alt="все четко можно мерге арго тест" src="https://github.com/user-attachments/assets/efbce9bc-3cb6-499f-ba6f-60653c27b645" />
<img width="1472" height="402" alt="синхронизация ок" src="https://github.com/user-attachments/assets/3088ce85-6bf1-4565-8f1b-7b0d5e2a324d" />

  * Наблюдаем изменения образа в DockerHub
<img width="1140" height="337" alt="изменения в образе" src="https://github.com/user-attachments/assets/fe9d09b0-0b8e-4788-8274-ebcf43567ba1" />

  * Проверяем конечную работу приложения
<img width="561" height="53" alt="изменения после внесения правок в докерфайл" src="https://github.com/user-attachments/assets/de81ff6a-4e84-42c5-aee6-d86ad2eba2f6" />

 








