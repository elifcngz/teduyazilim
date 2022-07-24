# MERGE SORT PROJESİ


## Soru 1

| 16 | 21 |11 | 8 | 12 | 22 |
| :--- | :---: | ---: | :---: | ---: | ---: |

Merge Sort diziyi öncelikle iki parçaya ayırarak işimizi kolaylaştırmayı ve hızlı olmayı amaçlar.Bu nedenle [16,21,11,8,12,22] dizimizi ikiye ayırarak işe başlamalıyız.

- Dizimiz,

| 16 | 21 |11 | 
| :--- | :---: | ---: |    

ve   


| 8 | 12 |22 | 
| :--- | :---: | ---: | 

olarak ikiye ayrılır.


- Daha sonra iikiye ayrılan bu iki küçük dize de kendi aralarında ikiye ayrılır.Bu nedenle 

 | 16 | 21 |11 | 
| :--- | :---: | ---: |   

dizisi   

 | 16 |  ve   |  21   11  | şeklinde ikiye bölünebilir.(Tam bölünmediğinde hangi tarafa fazla veri geldiğinin önemi yoktur.)

 - Aynı şekilde 

| 8 | 12 |22 | 
| :--- | :---: | ---: | 

dizisi de 

| 8  |   ve  |  12   22  | şeklinde ikiye ayrılabilir.


- Bir sonraki adımda yine tek olan veriler tek şekilde devam ederken | 21  11 |  ve  |  12  22  | dizeleri de tek tek ayrılır. Kısacası hepsi tek olana dek ikiye bölme işlemi gerçekleştirilir.

-  Bir sonraki adımda ayırdığımız | 21  11 | dizisi  | 11  21 | şeklinde sıralı olarak tekrar birleştirilir. Aynı şekilde |  12  22  | dizisi |  12  22  | olarak tekrar biraraya gelirler. 

- Böylece elimizde bir tarafta |  16  | ve  | 11  21  | dizileri, diğer tarafta ise |  8  | ve |  12  22  | dizileri bulunmaktadır.

-Bu dizileri de tekrar sıralı bir şekilde birleştirmemiz gerekir. Ve birleştirdiğimizde elimizde

| 16 | 11 |21 | 
| :--- | :---: | ---: |  

ve 

| 8 | 12 |  22 | 
| :--- | :---: | ---: |  

dizileri sıralanmış halde bulunmuş olur.

- Son olarak bu dizileri de tekrar sıralı bir şekilde birleştirdiğimizde 

| 8 | 11 |12 | 16 | 21 | 22 |
| :--- | :---: | ---: | :---: | ---: | ---: |

sıralı dizisini elde ermiş oluruz. Merge Sort ile insertion sorta göre daha hızlı bir şekilde işlemlerimizi bitirmiş oluruz.


## Soru 2

Big-O gösterimi tekrar eden bir işlem olduğu ve her seferinde işlemleri ikiye bölerek devam ettiği için 2^x=n şeklinde devam eden bir yapıya sahiptir. Bu nedenle merge sort işlemi için dizinin uzunluğu olan n(tekrar etme sayısını gösterir burada) ile 2^x=n işleminin diğer bir tanımlaması olan logn kullanılmış olur. Böylece merge sort için dizilerin big-O gösterimi  O(nlogn) şeklinde olur. Bizim sorumuzda 6 tane verimiz olduğu için big-O gösteriöi O(6log6) ifadesi ile gösterilebilir.







	                                 		