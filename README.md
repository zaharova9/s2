# s2
Есть 3 таблицы с артикулами товаров. Для каждой таблицы заменить колонку с идентификаторами так, чтобы в каждом новом файле номер продолжался с последнего из предыдущего файла. Используйте библиотеку pandas.
import pandas as pd

# использовать функцию с xlsx
df = pd.read_excel('1.xlsx', sheet_name='Лист1')
print(df.head())
df = pd.read_excel('2.xlsx', sheet_name='Лист1')
print(df.head())
df = pd.read_excel('3.xlsx', sheet_name='Лист1')
print(df.head())

# def replace_ids(filename,start_id):
#   data = pd.read_csv(filename) 
  
# # чтение данных из CSV файла
# data['id'] = data.index + start_id
# # создание новой колонки 'id' с новыми идентификаторами
# data.to_csv(filename,index=False)
# # запись данных обратно в CSV файл

# file1 = 'фйл1.csv'
# start_id1 = 1
# file2 = 'Копия2.csv'
# start_id2 = 100
# file3 = 'Копия3.csv'
# start_id3 = 200

# replace_ids(file1,start_id1)
# replace_ids(file2, start_id2)
# replace_ids(file3, start_id3)
