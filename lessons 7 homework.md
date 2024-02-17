first_list = []
while True:
    user = input('enter your number or stop:')
    if user.lower() == 'stop':
        break
    first_list.append(int(user))
print('first list:', first_list)
second_list = []
for i in first_list:
    if i % 2 == 0:
        second_list.append(i)
    list_second_copy = second_list.copy()
print('list_first:', first_list)
print('second_list:', second_list)

to_do=[]
print('додати завдання:')
while True:
    chores=input('>')
    if chores=='q':
        break
    else:
        to_do.append(chores)
print('завдання на сьогодні:')
for i in range(len(to_do)):
    to_do.sort()
    print(f'{i+1}.{to_do[i]}')


print("видалені завдання на сьогодні")
to_do.pop(2)
print(to_do)
