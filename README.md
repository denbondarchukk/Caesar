# Чат-бот для відповідей на деякі запитання зі шкільної програми

## Опис
Програма написана на мові Python і включає в себе різноманітні функції, які взаємодіють з користувачем через консоль.

## Вимоги
- Python 3.x
- Стандартні бібліотеки: `datetime`, `random`, `math`

## Використання

1. Завантажте або скопіюйте репозиторій.
2. Запустіть програму у вашому середовищі Python.

## Можливості розширення тематики

### Приєднання основної теми

Щоб додати основну тему (наприклад, "історія"), впишіть цю тему в лапках у словник `topics_dictionary` і поставте двокрапку з подвійними фігурними дужками:

```python
topics_dictionary = {
    "історія": {}
}
```

## Приєднання підтеми до основної теми
Для додавання підтеми впишіть цю підтему в лапках у фігурні дужки теми, до якої вона відноситься (наприклад, підтема "місто з найбільшою кількістю населення" буде в темі "географія"):
```python
topics_dictionary = {
    "географія": {
        "місто з найбільшою кількістю населення": {}
    }
}
```
Після цього необхідно створити функцію, в якій бот відповідатиме на це питання:
```python
def largest_city_by_population():
    response = "Токіо є містом з найбільшою кількістю населення у світі."
    print_response(response)
```
## Приєднання підтеми до підтеми
У такому випадку впишіть цю підтему в лапках у фігурні дужки підтеми (наприклад, "квадрат" буде в підтемі "обчислення площі" теми "математика"):
```python
topics_dictionary = {
    "математика": {
        "обчислення площі": {
            "квадрат": {}
        }
    }
}
```
Далі створіть функцію з рішенням:
```python
def calculate_square_area():
    a = get_float_input("Введіть сторону квадрата: ")
    area = a * a
    response = f"Площа квадрата зі стороною {a} дорівнює {area}."
    print_response(response)
```




