## [16, 21, 11, 8, 12, 22] dizisinin merge sort türüne göre aşamalarını yazınız.
Merge sort'a göre, diziyi tek eleman kalana kadar ikiye bölerek başlıyoruz. Sonrasında tüm tek elemanları ikili ve sıralı bir biçimde birleştiriyoruz. Oluşan listelere de aynı işlemleri uyguluyoruz.
|            |           |
|------------|-----------|
|[16, 21, 11]|[8, 12, 22]|
|[16, 21]|[11]|[8]|[12, 22]|
|[16]|[21]|[11]|[8]|[12]|[22]|
|[16, 21]|[8]|[11]|[12, 22]|
|[16, 21, 8]|[11, 12, 22]|
|Sort sonucu(son adım)|[8, 11, 12, 16, 22]|

## Big-O gösterimini yazınız.
Merge sort yaparken n tane elemana ikiye bölme işlemi yaptık. 2^x = n işleminde x sayısı bize kaç kere 2'ye böldüğümüzü gösteriyor. Bulmak için x = log(n) işlemini yapıyoruz, elbette 2 tabanında ancak bir gösterim bulmayı amaçladığımız için o çok da önemli değil. Buradan O(log(n)) elde ediyoruz. Böldükten sonra n eleman için sıralama yaptığımızdan Big-O gösterimi olarak O(nlog(n)) elde etmiş oluyoruz.

[patika](www.patika.dev)
