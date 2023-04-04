# ulfa stevi juliana
# G1A022042
"""
Functional Programming (FP) dan Object-Oriented Programming (OOP)
adalah paradigma pemrograman yang berbeda dalam hal pendekatan dalam 
menyelesaikan masalah. Pada Python, kedua paradigma dapat digunakan untuk
membuat program, dan perbedaan utama antara keduanya adalah sebagai berikut:

1. Pendekatan
FP fokus pada fungsi atau pemetaan dari input ke output dan tidak bergantung
pada state. FP menganjurkan untuk menghindari efek samping (side-effect) 
seperti mengubah variabel global dan objek mutable. Sedangkan OOP lebih 
fokus pada objek dan perilaku atau method yang terkait dengan objek tersebut.

2. Keuntungan
FP cenderung lebih mudah di-debug dan diuji karena fungsinya bersifat 
deterministik dan tidak bergantung pada state global. FP juga cenderung 
lebih mudah diparalelkan karena tidak ada masalah penjadwalan (scheduling) 
yang terkait dengan state. Sementara itu, OOP memungkinkan untuk menggabungkan 
data dan perilaku ke dalam satu entitas, sehingga lebih mudah untuk memodelkan 
dunia nyata yang kompleks.
"""

# Functional Programming (FP)
def square(num):
  return num ** 2

def map_square(numbers):
  return list(map(square, numbers))

numbers = [1, 2, 3, 4, 5]
squares = map_square(numbers)
print(squares)  #print : [1, 4, 9, 16, 25]
""""
Program di atas merupakan contoh program FP. 
Fungsi square adalah fungsi murni yang hanya mengambil input 
dan menghasilkan output tanpa efek samping. Fungsi map_square
adalah fungsi tingkat tinggi yang menggunakan fungsi map untuk
menerapkan fungsi square pada setiap elemen dari daftar numbers.
Akhirnya, hasilnya dicetak ke layar.
Dengan menggunakan paradigma FP dan fungsi bawaan Python map, 
kita dapat dengan mudah melakukan operasi pada setiap elemen dari 
suatu daftar/list tanpa harus melakukan loop secara eksplisit. 
Fungsi map akan menerapkan suatu fungsi pada setiap elemen dari 
suatu daftar/list, dan mengembalikan daftar/list yang berisi hasil 
operasi tersebut pada setiap elemen.
"""

# Object-Oriented Programming (OOP)
class Rectangle:
  def __init__(self, width, height):
    self.width = width
    self.height = height

  def area(self):
    return self.width * self.height

rectangle = Rectangle(10, 5)
print(rectangle.area()) #print : 50
"""
Program di atas merupakan contoh program OOP. 
Kelas Rectangle mewakili entitas geometris dengan sifat 
lebar dan tinggi. Metode area di dalam kelas digunakan 
untuk menghitung luas dari objek Rectangle. Objek rectangle 
dibuat dengan menggunakan konstruktor Rectangle dan kemudian 
metode area dipanggil pada objek untuk menghitung luasnya.
"""
