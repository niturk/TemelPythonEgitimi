# Donguler
[Geri](6-kararyapilari.md)
#### For Dongusu
```python
liste = ['elma', 'armut', 'muz', 'ananas']

for meyve in liste
    print(meyve)


sayi_liste = [1,2,3,4,5,6,7,8,9]
for sayi in sayi_liste:
    if sayi % 2 == 1:
        print(sayi)

dict = {
    'k1': 1,
    'k2': 2,
    'k3': 3
}
for key,value in dict.items():
    print(key,value)

for key in dict.keys():
    print(key)

for value in dict.values():
    print(value)
```

#### While Dongusu
```python
# Boolean tabanli dongu.
i = 0
while i < 5:
    print(f'i = {i}')
    i = i + 1
else:
    print('i 5 ten kucuk degil.')
```

* sonsuz dongu
```python
while True:
    print('Sonsuzda bitecek, cok birsey kalmadi az bekle.')
```

#### Break / Continue / Pass
```python
break: Donguyu kirarak devam eder.
continue: Dongunun ilgili adimini es gecer.
pass: Yer tutucu olarak kullanilir. Etkisizdir.
```

#### Ornekler
```python
for num in range(10):
    print(num)

for num in range(0,10,2):
    print(num)
```

* zip
```python
meyveler = ['elma', 'armut','muz']
fiyatlar = [5,7,20]

urunler = zip(meyveler, fiyatlar)
urun_list = list(urunler)
print(urun_list)

for urun in urun_list:
    print(urun)

for index,urun in enumerate(urun_list):
    print(index, urun)
```

* min / max
```python
num_list = [1,10,50,70,2,80,5,200,300,6]
print(max(num_list))
print(min(num_list))
```

* random
```python
from random import shuffle
num_list = [1,2,3,4,5,6,7,8,9,10]
shuffle(num_list)
print(num_list)

from random import randint
rastgele_sayi = randint(0,100)
print(rastgele_sayi)
```

* Pythonic
```python
# 1. yontem
mylist = list()
for x in range(0, 100):
    if x%2 == 0:
        mylist.append(x**2)
print(mylist)

# Pythonic
mylist = [x**2 for x in range(0,100) if x%2 == 0]
```

[Metodlar ve Fonksiyonlar](8-methodfunctions.md)