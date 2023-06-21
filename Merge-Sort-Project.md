# [16,21,11,8,12,22]-Merge Sort

1. Küçükten büyüğe sıralamak için ilk adım olarak diziyi eşit iki parçaya ayırıyoru: [16,21,11] ve [8,12,22]
2. Oluşan dizileri tek eleman kalana kadar tekrar ikiye ayırıyoruz: [16,21], [11] & [8,12], [22]
3. [16], [21], [11] & [8], [12], [22]
4. Kendi aralarında sıralı olacak şekilde elemanları karşılaştırarak tekrar birleştiriyoruz: [16,21], [11] & [8,12], [22]
5. Tekrar aynı işlemi yapıyoruz: [11,16,21] & [8,12,22]
6. [8,11,12,16,21,22]

 **Big O**=> Her birleştirme işleminde n-1 işlem yapıldığı için time complexity O(n), bu işlemi kaç defa terarlıyoruz? 2^x=n, x=logn. O(n) time complexity, logn kere yapıldığı için bütün işlem için **Big O Notation= nlogn** oluyor.  