# Metodlar ve Fonksiyonlar
[Geri](7-donguler.md)
## Metodlar

```python
num_list = [1,2,3,4]

num_list.append(5)

print(num_list)
help(num_list.append)
```

https://docs.python.org/3.8/library/

## Fonksiyonlar
```python
#f(x) = 2x + 1
#f(x) = y

def f(x):
    return 2 * x + 1

# parametresiz fonksiyon
# return olan fonksiyonlar
def f():
    return 5

# print(yaz(x))
# return olmayan fonksiyonlar
def yaz(x):
    print(x)

f(1) # 2 * 1 + 1 = 3
f(2) # 2 * 2 + 1 = 5

print('Ders bitmek uzere.')
yaz('Ders bitmek uzere.')
```
* deger donduden ve dondurmeyen fonksiyonlar
```python
def toplama_islemi_yap(sayi1, sayi2):
    return sayi1 + sayi2

def toplama_sonucu_yazdir(sayi1, sayi2):
    print(sayi1 + sayi2)

def topla_ve_ayni_zamanda_yazdir(sayi1, sayi2):
    sonuc = sayi1 + sayi2
    print(sonuc)
    return sonuc

```python
# moduller, kutuphaneler
import time

def yas_hesapla(dogum_yili):
    yas = suanki_yil - dogum_yili
    return yas

# simdiki yili bul
suanki_yil = int(time.strftime("%Y"))

# dogum tarihini iste
dogum_tarihi = int(input('Dogum tarihinizi giriniz.'))

yas = yas_hesapla(dogum_tarihi)

print(yas)
```

* varsayilan parametre
```python
def merhaba(isim='Varsayilan'):
    print(f'Merhaba {isim}')

merhaba('Nikita')
```

* ornekler
```python
def cift_sayi_mi(sayi):
    return sayi % 2 == 0

if cift_sayi_mi(5):
    print('Cift')
else:
    print('Tek')
```

### Local Modul Kullanimi

`modulum.py`
```python
def toplama(x,y):
    return x + y
def cikarma(x,y):
    return x - y
def carpma(x,y):
    return x * y
def bolme(x,y):
    return x / y
```

`main.py`
```python
from modulum import bolme, carpma, cikarma, toplama

sayi1 = 10
sayi2 = 10

sonuc = toplama(sayi1, sayi2)

print(sonuc)
```

[Hata Yakalama](9-hatalar.md)