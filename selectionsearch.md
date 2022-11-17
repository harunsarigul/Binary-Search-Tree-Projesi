Selection Sort Projesi
[22,27,16,2,18,6] -> Insertion Sort 

<!-- Yukarı verilen dizinin sort türüne göre aşamalarını yazınız. -->
<!-- Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız -->
<!-- Average case: Aradığımız sayının ortada olması 
     Worst case: Aradığımız sayının sonda olması
     Best case: Aradığımız sayının dizinin en başında olması. -->

      0 - [22,27,16,2,18,6]
      1-  [2,27,16,22,18,6]  
        <!--  {en küçük elemanı buluyor(2) ve 1. sıradaki sayı ile(22) yer değiştiriyor -->
      2-  [2,6,16,22,18,27] 
        <!-- {2 den sonraki en küçük sayıyı buluyor(6) ve 2. sıraki sayı ile yer değiştiriyor -->
      3-  [2,6,16,18,22,27] 
        <!-- {3. en küçük sayı(16) zaten doğru yerinde olduğu için hiç dokunmayıp 4. en küçük sayıyı 4. sıradaki sayı ile yer değişiyor. -->
      4-  [2,6,16,18,22,27]
        <!-- dizi sıralı bir şekilde son halini alıyor -->


         Dizideki eleman sayısı n olursa ilk adımda n eleman kadar inceleyip en küçüğünü başa yazarız. İkinci adımda kalan (n-1)  eleman kadar , üçüncü adımda ise (n-2) eleman kadar 
        inceleriz ve 1 elemana kalana kadar bu işlemi tekrarlarız.
             
         Fonksiyonumuz "n+(n-1)+(n-2)...+1" den " (n*(n+1)) / 2 " olur. Big-O gösterimi için fonksiyonu domine eden kısım alınır.

             Big-O gösterimi O(n^2) şeklindedir.

             Time Complexity: Dizi sıralandıktan sonra 18 sayısı dizinin ortasında yer alır. Bu yüzden Average case'e girer.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

 [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

      0- [7,3,5,8,2,9,4,15,6] 
      1- [2,3,5,8,7,9,4,15,6] 
      2- [2,3,4,8,7,9,5,15,6] 
      3- [2,3,4,5,7,9,8,15,6] 
      4- [2,3,4,5,6,9,8,15,7] 
      . 
      . 
