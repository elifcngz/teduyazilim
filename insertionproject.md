# Intersection Sort Project

## Soru 1




* Insertion Sort linear bir şekilde ilerleyerek bir listeyi sıralamamızı sağlar.Verilen örüntüye ait en küçük elemanı buluyor ve en baştaki sayı ile yer değiştiriyor. Peki ya devamı? İkinci en küçük elemanı buluyor ve 2. sıra ile değiştiriyor. Bu şekilde sıralı hale gelene kadar devam ederek sıralamayı tamamlamış oluyoruz. 
Sıralamamız ilk hali:

| 22 | 27 |16 | 2 | 18 | 6 |
| :--- | :---: | ---: | :---: | ---: | ---: |




- İlk olarak ilk verimiz olan 22 ile en küçük verimizi olan 2'in yerlerini değiştireceğiz.


| ***2*** | 27 |16 | ***22*** | 18 | 6 |
| :--- | :---: | ---: | :---: | ---: | ---: |

- Daha sonra 2. verimiz olan 27 ile geri kalan kısımdaki en küçük verimiz olan 6'nın yerini değiştirmemiz gerekiyor.

| 2 | ***6*** |16 | 22 | 18 | ***27*** |
| :--- | :---: | ---: | :---: | ---: | ---: |

- Diğer adımımızda ilk iki verimiz sıralandığı için 3. verimize bakarız, geri kalan kısımdaki sayılardan küçük olduğu için aynı yerinde kalır.

| 2 | 6 | ***16*** | 22 | 18 | 27 |
| :--- | :---: | ---: | :---: | ---: | ---: |

- Daha sonra 4. verimiz olan 22 ile kendisinden küçük olan 18'in yerini değiştirmemiz gerekir.

| 2 | 6 | 16 | ***18*** | ***22*** | 27 |
| :--- | :---: | ---: | :---: | ---: | ---: |

- Sonunda verilerimiz üçükten büyüğe doğru insertion sort yöntemi ile sıralanmış hale geldi.










## Soru 2

[22,27,16,2,18,6] dizisi sırasız bir dizi bu nedenle iki kere tekrarlama gösterir. Big-O gösterimi O(n^2) şeklindedir.


## Soru 3

* 2.soruda da söylediğimiz gibi iki çevrimde gerçekleşir bu yüzden average ve worst caselerde durum aşağıdaki gibidir:

- Average Case: O(n^2)
- Worst Case: O(n^2)

* Ancak best case kısmında dizimiz en iyi ihtimalle sıralı olacağı için tek çevrim gerçekleşir. Bu durumda big-O gösterimi aşağıdaki şekildedir:

- Best Case: O(n)



## Soru 4

Dizimizin ilk hali

| 7 | 3 | 5 | 8 | 2 | 9 | 4 | 15 | 6 |
| :--- | :---: | ---: | :---: | ---: | ---: |:---: | ---: | ---: |
 
şeklindedir.






Insertion Sort'a göre dizimizin ilk 4 aşaması aşağıdaki gibidir:


- İlk olarak ilk verimiz olan 7 ile en küçük verimiz olan 2'nin yerini değiştirmekle işe başlamalıyız.


| ***2*** | 3 | 5 | 8 | ***7*** | 9 | 4 | 15 | 6 |
| :--- | :---: | ---: | :---: | ---: | ---: |:---: | ---: | ---: |


- Daha sonra ikinci verimize baktığımızda kalan verilerden küçük olduğu için aynı yerinde kalır. Bu yüzden 3. verimize bakmamız gerekir. 3. verimiz 5 ise 4 ile yer değiştirmelidir.



| 2 | 3 | ***4*** | 8 | 7 | 9 | ***5*** | 15 | 6 |
| :--- | :---: | ---: | :---: | ---: | ---: |:---: | ---: | ---: |


- Bu aşamada ise 4. verimize bakmamız gerekir. Buradaki 8 ile 5'nin yer değiştirmesi gerekir.



| 2 | 3 | 4 | ***5*** | 7 | 9 | ***8*** | 15 | 6 |
| :--- | :---: | ---: | :---: | ---: | ---: |:---: | ---: | ---: |


- 4.aşamamızda ise sıralı olması için 5. verimiz olan 7 ile 6'nın yer değiştirmesi gerekir.




| 2 | 3 | 4 | 5 | ***6*** | 9 | 8 | 15 | ***7*** |
| :--- | :---: | ---: | :---: | ---: | ---: |:---: | ---: | ---: |

Böylece soruda istenen Insertion Sort'a göre olan 4 aşamayı göstermiş olduk.

