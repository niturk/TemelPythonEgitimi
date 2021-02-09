# Hata Yakalama
[Geri](8-methodfunctions.md)

### Herhangi bir hatayi yakalamak

```python
try:
    sayi1 = 10
    sayi2 = 10

    sonuc = sayi1 / sayi2
    print(sonuc)
except:
    print('Bilinmeyen bir hata olustu.')
```

### Bilinen hatalari yakalamak

```python
try:
    sayi1 = 10
    sayi2 = 0

    sonuc = sayi1 / sayi2
    print(sonuc)
except ZeroDivisionError:
    print('2. sayi "0" olamaz. Sonuc tanimsizdir.')
except:
    print('Bilinmeyen bir hata olustu.')
```

* ornek
```python
# Kullaniciyi integer bir sayi vermeye zorlayalim.

def kullanicidan_sayi_al():
    while True:
        try:
            kullanicidan_gelen = input('Lutfen bir sayi giriniz.')
            alinan_sayi = int(kullanicidan_gelen)
        except:
            print('Lutfen ama sayi istemistim')
            continue
        else:
            print(f'Tesekkurler, {alinan_sayi} uygun.')
            break

sayi = kullanicidan_sayi_al()
```