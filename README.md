## API Testing для приложения Яндекс.Прилавок

### Контекст и ссылки
- **Требования API:** [Ссылка на документацию](https://code.s3.yandex.net/qa/files/backend_requirements.pdf)

### Предусловия к тестированию

Изучить новую функциональность.

**1. Работа с наборами**
- возможность добавлять продукты в набор — ручка POST /api/v1/kits/{id}/products
  
**2. Работа с курьерами**
- возможность проверить, есть ли доставка курьерской службой «Привезём быстро» и сколько она стоит. Ручка POST /fast-delivery/v3.1.1/calculate-delivery.xml
  
**3. Работа с корзиной**
- возможность получить список продуктов, которые добавили в корзину. Ручка GET /api/v1/orders/:id
- возможность добавлять продукты в корзину. Ручка PUT /api/v1/orders/:id
- возможность удалять корзину. Ручка DELETE/api/v1/orders/:id

### Задачи

**1. Функциональное тестирование API**
- Тестирование всех методов API (GET, POST, PUT, DELETE)
- Проверка кодов ответа и статусов
- Валидация JSON-схем ответов

**2. Позитивные и негативные сценарии**
- Проверка валидных запросов с корректными данными
- Тестирование обработки невалидных данных и ошибок
- Проверка граничных значений параметров

### Результаты работы

**Тестирование API:**
- Чек-лист тестирования: [Ссылка на таблицу](https://docs.google.com/spreadsheets/d/1txjDULOCZWeizQtvwhRL91lqNOkER6tR0uEROYjuMEw/edit?usp=sharing)
  
![Скриншот чек-листа](https://github.com/user-attachments/assets/68e9b955-2a32-491a-8cbf-727312893bfb)
![Скриншот чек-листа лист2](https://github.com/user-attachments/assets/e7bd31e5-33db-42e2-aa32-32d5a6f94a24)

- Баг-репорты: [Ссылка на таблицу с багами](https://docs.google.com/spreadsheets/d/1txjDULOCZWeizQtvwhRL91lqNOkER6tR0uEROYjuMEw/edit?gid=1190841100#gid=1190841100)

![Скриншот баг-репорт лист1](https://github.com/user-attachments/assets/a632e515-ca5f-41ac-a07c-ea190ddbd1c4)
![Скриншот баг-репорт лист2](https://github.com/user-attachments/assets/bd134749-8309-4a99-b82e-988831f9c4d6)
![Скриншот баг-репорт лист2](https://github.com/user-attachments/assets/7811c4b9-2cd5-4259-8ec3-277bd911d4ff)
