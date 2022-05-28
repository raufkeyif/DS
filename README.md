# DS
Merge sort Projesi
##  **MERGE SORT PROJESİ**

[16,21,11,8,12,22] -> Merge Sort

● Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
-Öncelikle, Merge Sort'umuzu ikiye bölüyoruz. (İkiye tam bölünmek zorunda değil)

                   [16,21,11]   [8,12,22]
Ardından soldaki ve sağdaki dizileri tekrardan bölüyoruz.

            [16,21] [11]                        [8] [12,22]
tek eleman kalana kadar bir kez daha bölüyoruz.

        [16] [21] [11]                              [8] [12] [22]
 Bölme işlemi bitti. Şimdi sıralı bir dizi elde edinceye kadar birleştirme işlemine devam ediyoruz. (Küçükten büyüğe doğru sıralanmalı)
 
                  [16] [21] [11]                   [8] [12] [22] 
Şimdi İkili şekilde sıralayalım. 

                  [11,16] [21]                   [8,12] [22]
Ve son! en soldaki sayıları birbiri ile karşılaştırıp dizimize ekleyeceğiz.

                       [8,11,12,16,21,22]

●Aynı Dizinin, Big-o gösterimini yapalım
    
-   Diziyi parçalara ayırırken sürekli 2'ye böldüğümüz için; 2^x = n => logn,
-   Birleştirme yaparken ise elemanların birbirlerine göre karşılaştırmasını yapmanın maliyeti n - 1 => n,
-   Bütun bu işlemlerin maliyeti: O(n * logn)
