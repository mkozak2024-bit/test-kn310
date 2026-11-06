
def check_number(number):
    assert number > 0, "Число має бути більшим за нуль!"
    return number


def create_name(name):
    if not name:
        raise ValueError("Ім'я не може бути порожнім")
    return name


# Перевірка чисел
try:
    number = int(input("Введіть додатне число: "))
    print("Правильне число:", check_number(number))
except ValueError as error:
    print("Помилка:", error)
except AssertionError as error:
    print("Помилка:", error)
