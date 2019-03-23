# Это просто игра в камень, ножницы, бумага
import random

print ('__GAME__')
print ('Камень, Ножницы, Бумага')
app = int(random.randrange(1, 3,1))

print ('1) Камень')
print ('2) Ножницы')
print ('3) Бумага')
otv = 0

while otv != 'Стоп': 
    x = int (input (': '))
    if x == app:
	    print ('Ничья')
    elif (x == 1 and  app == 2) or (x == 2 and app == 3) or (x == 3 and app == 1):
	    print ("Ты выиграл")
    else: 
	    print ("Ты проиграл")
	  otv = input ('Продолжаем? Если хотите выйти введите "Стоп". Если хотите продолжить введите что угодно' )
