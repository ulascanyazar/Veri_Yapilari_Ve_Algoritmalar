## [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Binary search tree bir kökün (root) seçilmesiyle başlar. Seçilen root'un sol tarafında kendisinden küçük, sağ tarafında ise kendisinden büyük sayılar bulunur. Bu sayıların bulunduğu noktalara düğüm denir. Bu düğümler için de aynı sıralama koşulu geçerlidir.
Kökümüzü 7 seçelim.
|7|


5, 7'den küçük oldupu için soluna yerleştiriyoruz.


| | | |
|-|-|-|
| | |7|
| |/| |
|5| | |


1, hem 7'den hem de 5'ten küçük olduğu için şimdilik en sola yerleştiriyoruz.


| | | | | |
|-|-|-|-|-|
| | | | |7|
| | | |/| |
| | |5| | |
| |/| | | |
|1| | | | |


8 sayısı 7'den büyük odluğu için sağ tarafına yerleştiriyoruz.


| | | | | | | |
|-|-|-|-|-|-|-|
| | | | |7| | |
| | | |/| |\| |
| | |5| | | |8|
| |/| | | | | |
|1| | | | | | |


3 sayısı 7 ve 5'ten küçük, ancak 1'den büyük. Bu yüzden 1'in sağına ekliyoruz.


| | | | | | | |
|-|-|-|-|-|-|-|
| | | | |7| | |
| | | |/| |\\| |
| | |5| | | |8|
| |/| | | | | |
|1| | | | | | |
| |\| | | | | |
| | |3| | | | |


6 sayısı 7'den küçük ancak 5'ten büyük olduğu için 5'in sağına yerleştiriyoruz.


| | | | | | | |
|-|-|-|-|-|-|-|
| | | | |7| | |
| | | |/| |\| |
| | |5| | | |8|
| |/| |\| | | |
|1| | | |6| | |
| |\| | | | | |
| | |3| | | | |


0 sayısı 1'den küçük olduğu için en sola ekliyoruz.


| | | | | | | | | |
|-|-|-|-|-|-|-|-|-|
| | | | | | |7| | |
| | | | | |/| |\| |
| | | | |5| | | |8|
| | | |/| |\| | | |
| | |1| | | |6| | |
| |/| |\| | | | | |
|0| | | |3| | | | |


9, 8'den büyük, o yüzden en sağa yerleştiriyoruz.


| | | | | | | | | | | |
|-|-|-|-|-|-|-|-|-|-|-|
| | | | | | |7| | | | |
| | | | | |/| |\| | | |
| | | | |5| | | |8| | |
| | | |/| |\| | | |\| |
| | |1| | | |6| | | |9|
| |/| |\| | | | | | | |
|0| | | |3| | | | | | |


4, 5'ten küçük ancak 3'ten büyük. 3'ün sağına ekliyoruz.


| | | | | | | | | | | |
|-|-|-|-|-|-|-|-|-|-|-|
| | | | | | |7| | | | |
| | | | | |/| |\| | | |
| | | | |5| | | |8| | |
| | | |/| |\| | | |\| |
| | |1| | | |6| | | |9|
| |/| |\| | | | | | | |
|0| | | |3| | | | | | |
| | | | | |\| | | | | |
| | | | | | |4| | | | |


2, 3'ten küçük olduğundan sağına ekliyoruz.


| | | | | | | | | | | |
|-|-|-|-|-|-|-|-|-|-|-|
| | | | | | |7| | | | |
| | | | | |/| |\| | | |
| | | | |5| | | |8| | |
| | | |/| |\| | | |\| |
| | |1| | | |6| | | |9|
| |/| |\| | | | | | | |
|0| | | |3| | | | | | |
| | | |/| |\| | | | | |
| | |2| | | |4| | | | |
