# Dosya Islemleri
[Geri](3-temeller.md)
### Dosya Islem Modlari
```
r  -> okuma
w  -> yazma
a  -> ekleme
r+ -> okuma ve yazma
w+ -> okuma ve yazma (var olan dosyanin uzerine yazar veya yeni olusturur.)  
```

#### Dosya Yazma
```python
# dosya yazma
dosya = open('rehber.txt', 'w')
dosya.write('Nikita')
dosya.close()
```

#### Dosyadan Okuma
```python
# dosya okuma
dosya = open('rehber.txt', 'r')
icerik = dosya.read()
print(icerik)

dosya.seek(0) # cursor basa getir.
icerik_list = dosya.readlines()
print(icerik_list)
```

[Karsilastirma Islemleri](5-karsilastirmaislemleri.md)