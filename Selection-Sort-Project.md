# [22,27,16,2,18,6]->Selection Sort

- [**2**,27,16,22,18,6]->dizinin tamamı taranır ve en küçük eleman bulunur. Bu dizide en küçük eleman 2 olduğu için en baştaki 22 ile yer değiştirir. (tüm elemanları kontrol ettiğim için n sayıda işlem)
- [2,**6**,16,22,18,27]-> dizinin kalanı taranır, ikinci en küçük 6 ile 27'nin yeri değiştirilir. İlk elemanın yeri belli olduğu için n-1 işlem.
- [2,6,**16**,22,18,27]-> dizinin kalanı taranır, 16 üçüncü en küçük eleman olduğu için yeri değiştirilmez. 2 ve 6 dahil edilmediği için n-2 işlem
- [2,6,16,**18**,22,27]-> dizinin kalanı taranır, 18 dördüncü en küçük eleman olduğu için 22 ile yer değiştirilir. n-3 işlem
- [2,6,16,18,**22**,27]-> dizinin kalanı taranır, 22 beşinci en küçük eleman ve beşinci sırada olduğu için yeri değiştirilmez. n-4 işlem
- [2,6,16,18,22,**27**]-> dizinin kalanı taranır, elimizde sadece 27 olduğu ve en büyük eleman olduğu için yeri değiştirilmez. n-5 işlem yani 6 eleman olduğu için 1 işlem

**Big O**-> n+(n-1)+(n-2)...+1-> n.(n+1)/2=(n^2+n)/2=O(n^2)

**time complexity**-> 18 elemanı sıralamadan sonra dizinin neredeyse ortasında yer aldığından **average case**'dir. 

# [7,3,5,8,2,9,4,15,6]-Selection Sort
1. [2,3,5,8,7,9,4,15,6]
2. [2,3,5,8,7,9,4,15,6]
3. [2,3,4,8,7,9,5,15,6]
4. [2,3,4,5,7,9,8,15,6]