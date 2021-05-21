# Python Kurulumu

# github.com/niturk/TemelPythonEgitimi
### Indirme Linkleri
[Python 3.8.10](https://www.python.org/downloads/release/python-3810/)

[Visual Studio Code](https://code.visualstudio.com/)

**! indir ama kurma okumaya devam et**

</br>

![Python Logo](https://www.python.org/static/img/python-logo.png)
## Kisaca Python
* Python nesneye dayali bir programlama dilidir. (Hersey bir nesnedir.)

![Nesne Yonelimli Programlama](img/oop.png)
* Acik kaynaklidir. (https://github.com/python)
* Python programlarının en büyük özelliklerinden birisi, C ve C++ gibi dillerin aksine, derlenmeye gerek olmadan çalıştırılabilmeleridir.
* Basit ve temiz söz dizimi bulunur kolay yazılır ve okunur.
```python
print("Merhaba Dunya")
```
* Python 2 vs 3 (Python 2 bazi uygulamalar hala kullaniyor.)
* Uyumlu heryerde calisir.
    - Elektronik - Micropython (https://micropython.org/)
    - Web - Django, Flask (https://www.djangoproject.com/)
    - Mobil - Kivy (https://kivy.org/#home)
    - Desktop GUI - PySide2 (https://wiki.qt.io/Qt_for_Python)
    - Devops - Ansible (https://www.ansible.com/)
    - Veri Bilimi - Numpy/Pandas (https://numpy.org/)
    - Görüntü İşleme - OpenCV (https://opencv.org/)
    - Ses ve Video Isleme - scikit-video (http://www.scikit-video.org/stable/)
    - Yapay Zeka ve Makina Ogrenmesi - Keras, SciPy, Pandas, TensorFlow (https://keras.io/)
    - Web Scrapping Uygulamalari - Selenium,BeautifulSoup (https://www.selenium.dev/)
* Awesome Python (https://awesome-python.com/)
* Real Python (https://realpython.com/)
* PyPi (https://pypi.org/)
* Python Pratikler (https://book.pythontips.com/en/latest/index.html)
* Full Stack Python (https://www.fullstackpython.com/)
* Test Driven Development Course (https://testdriven.io/)
* Turkce Kaynak (https://python-istihza.yazbel.com/)
* Dropbox, Instagram, Amazon, Pinterest, Netflix, Spotify, Facebook, Youtube, Udemy
* Komplek sistemlerde birden fazla programlama dili kullanilabilir. Python ile C/C++ fonksiyonlarina binding islemi yapilabilir.

* `ctypes` (https://docs.python.org/3.8/library/ctypes.html#loading-shared-libraries)

![Python You Can Fly](img/python-fly.jpeg)

![Github Ranking](img/github_ranking.png)
Github Ranking
### C vs Python
Python Kodu
```python
print('Hello, World!')
```
C Kodu
```c
#include <stdio.h>
int main()
{
  printf("Hello, World!");
  return 0;
}
```
#### **Daha iyi bir ornek**

Python Kodu
```python
# python
year = 2021
print('Merhaba İZÜ!')
print(f"{year} Yılındayız.")
```
```python
python program.py
```
C Kodu
```c
// c
#include <stdio.h>

int main() {
	int year = 2021;
	printf("Merhaba İZU!\n")
	printf("%d Yilindayiz.\n", year);
	return 0;
}
```
```shell
gcc c_programi.c -o programAdi
./programAdi
```

## Python 3.8 Kurulumu

https://www.python.org/downloads/

* Kullanilacak Surum : Python 3.8

**Add Python 3.8 to PATH secilmelidir!**

![Python Path](img/pythonpath.png)



* Kurulum basarili.

![Python Interpreter](img/pythoninterpreter.png)

#### Kod yazarken kullanacağımız yardımcılar

Formatter [black] -> https://github.com/psf/black
* Pep kurallarina gore kodu duzenler.

![Pep8 Apartman](img/pep8-apartman.jpg)

![Auto Pep8](img/auto-pep8.png)

Linter [flake8] -> https://github.com/PyCQA/flake8
* Kod hatalarini soyler.
* Orn. kullanilmayan bir kutuphane cagirildiginda.

### Paket Kurulumu

[PyPI Python Paketleri](https://pypi.org/)

`pip` yazilimi kullanilarak yapilir.
```python
pip install paket_adi
```

### Paket Yoneticisi : Pipenv Kurulumu

https://pipenv-fork.readthedocs.io/en/latest/

```shell
pip3 install pipenv
```

## Editor - Ide

* PyCharm - (https://www.jetbrains.com/pycharm/)
* [Visual Studio Code](2-vscode.md)
* Atom - (https://atom.io/)
