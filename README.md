# Homework_12

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Ex.1

Дана строка, в которой буква h встречается минимум два раза. Удалите из этой строки первое и последнее вхождение буквы h, а также все символы, находящиеся между ними.

def remove_h(input_h):
    first_h = input_h.find('h')
    last_h = input_h.rfind('h')   
    if first_h != -1 and last_h != -1:
        result_str = input_h[:first_h] + input_h[last_h + 1:]
        return result_str
    else:
        return input_h
input_string = "ahaaaha"
result = remove_h(input_string)
print(result)

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Ex.2

Создайте словарь всех покупателей и стоимости покупок (для каждого покупателя: стоимость покупки). найти для такого словаря:
    • максимальную стоимость покупки и кто совершил эту покупку
    • кол-во сделанных продаж

    # purchases = {
#     'Покупатель номер 1': 150,
#     'Покупатель номер 2': 200,
#     'Покупатель номер 3': 130,
#     'Покупатель номер 4': 250,
#     'Покупатель номер 5': 180
# }
# Max_purchase = max(purchases, key=purchases.get)
# Max_cost = purchases[Max_purchase]
# print(f"Максимальная стоимость покупки: {Max_cost} у {Max_purchase}")
# Number_of_sales = len(purchases)
# print(f"Общее количество продаж: {Number_of_sales}")


