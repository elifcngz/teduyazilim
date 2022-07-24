# BINARY SEARCH TREE PROJESİ

## Soru 1

    - Bir düğüm her iki tarafa da referans verebiliyor. Sağ ve sol olarak. Sağ tarafından kendinden büyük elemanlar, sol tarafında ise kendinden küçük elemanlar bulunacak.

    -AŞAMA 1:
    Öncelikle 7 rootumuz olsun diyerek başlayabiliriz.

    -AŞAMA 2:
    Daha sonra 5 ve 8 sayılarını ele alalım. 5 ifadesi 7'den küçük olduğu için ağacın sol tarafına, 8 ifadesi ise 7'den küçük olduğu için ağacın sağ tarafına yazılmalıdır.

                                           |7|

                                    |5|           |8|

   - Aşama 3:
   Bu aşamada ise 5 ve 8 ifadelerinim sağına ve soluna yazabileceğimiz  ifadeleri seçeceğiz.
   1 , 5'ten küçük oldğu için 5'in soluna yazılırken 6 5'ten büyük olduğu için sağına yazılır.
   Aynı şekilde 8 için de değerlendirdiğimizde 9'u sağ tarafa yazabiliriz.

                                           |7|

                                    |5|           |8|

                            |1|          |6|           |9|


-Aşama 4: 
  Geriye kalan 0,3,2 v3 4'ün tamamı 7'den zaten küçük olduğu için 8'e uzanan dalla işimiz bitmiştir diyebiliriz.
  0, 1'den küçük olduğu için soluna, 3 1'den büyük olduğu için sağına yazılmalıdır.


                                         |7|

                                    |5|           |8|

                            |1|          |6|           |9|

                        |0|     |3|

-Aşama 5: 
Son aşamamızda ise 2 ve 4'ün yerlerini belirlememiz gerekir. 2, 3'ten küçük olduğu için sol tarafına, 4 büyük olduğu için  sağ tarafına yazılır.


                                         |7|

                                    |5|           |8|

                            |1|          |6|           |9|

                      |0|         |3|
                              
                               |2|    |4|

Böylece binary search ağacımızı tamamlamış oluruz.