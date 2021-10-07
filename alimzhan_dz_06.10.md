#alimzhandunenov
# alimzhan
ZADANIE 1

duration = int(input('Введите количество секунд'))
if duration < 60:
    print(duration, 'сек')
elif 3600 > duration >= 60:
    min = duration // 60
    sec = duration % 60
    print(min, 'мин', sec, 'сек')
elif 86400 > duration >= 3600:
    min = (duration//60) % 60
    sec = duration % 60
    h = duration // 3600
    print(h, 'ч', min, 'мин', sec, 'сек')
elif 2629743 > duration >= 86400:
    min = (duration//60) % 60
    sec = duration % 60
    h = duration % 86400 // 3600
    d = duration // 86400
    print(d, 'д', h, 'ч', min, 'мин', sec, 'сек')
elif 31556926 > duration >= 604800:
    min = (duration//60) % 60
    sec = duration % 60
    h = duration % 86400 // 3600
    d = duration % 604800 //86400
    w = duration // 2629743
    print(w, 'мес',d, 'д', h, 'ч', min, 'мин', sec, 'сек')
    
    ///////////////////////////////////////////////////////
    ZADANIE 3
    
    list_one = list(range(21, 92, 10)) + [1]
list_two = list(range(2, 5))
list_three = list(range(11, 15))
n = 1
end = n % 10
while n <= 100:
    if n in list_three:
        print(n, 'процентов')
        n += 1
        end = n % 10
    elif end in list_two:
        print(n, 'процента')
        n += 1
        end = n % 10
    elif end in list_one:
        print(n, 'процент')
        n += 1
        end = n % 10
    else:
        print(n, 'процентов')
        n += 1
        end = n % 10
