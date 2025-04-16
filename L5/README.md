## Лабораторная работа №5

**Интеграционное тестирование. Тестирование веб-API**

**Цель работы:** изучить основные особенности интеграционного тестирования. Получить базовые практические навыки по тестированию и документированию веб-*API* с использованием *Postman*.
 
### Задание

Разработать тесты и документацию для *RESTful*-сервиса, разработанного по дисциплине ПРКИСОТ (л.р. №4), с использованием [Postman](https://www.postman.com/downloads/). Тесты должны покрывать все открытые методы *API* со всеми возможными вариантами входных данных.

*При написании тестов в Postman базово необходимо проверять статус-код HTTP-ответа. Если метод сервиса возвращает данные в формате JSON, то также необходимо сначала проверить правильность структуры JSON, а затем проверить значения полей.*

Требования к документации:
- описание к методам должно быть кратким, четким и понятным
- должны быть описаны входные параметры: тип и допустимые значения
- должны быть описаны возвращаемые методом статус-коды и их обозначение. Если метод возвращает данные в формате _JSON_, то должна быть описана его структура
- для описания документации использовать формат _Markdown_

**Разрешается (даже рекомендуется) оформить документацию на английском языке**

---
**Пример описания метода:** `GET /groups/{id}`
Data for a specific group.

**Params:**
- `id` - ID of the group (`integer`, `> 0`)

**Success response:**
Code: `200 OK`
Content-Type: `application/json`
Body:
- `id` - ID of the group (`integer`)
- `name` - name of the group (`string`)
- `students` - array of students (see _Student API_)
    - `id` - ID of the student (`integer`)
    - `lastName` - last name of the student (`string`)
    - `firstName` - first name of the student (`string`)

**Error response:**
Code: `400 Bad request`
If `id` is wrong or group with this `id` does not exist.
---

### Дополнительно

[Базовая теория по _Postman_](https://github.com/the-hwk/GSTU-software-testing/blob/main/L5/postman-base-theory.pdf)
