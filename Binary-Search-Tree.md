# [7,5,1,8,3,6,0,9,4,2]-Binary Search Tree
1. İlk elemanımız 7 olduğu için root'umuz 7 oluyor. 
2. İkinci eleman 5<7 olduğu için rootun solunda yer alacak.
3. Üçüncü eleman 1<7 olduğu için bir alttaki node'a bakıyoruz. 1<5 olduğu için 5'in soluna yazılır.
4. Dördüncü eleman 8>7 olduğu için 7'nin sağına yazılır.
5. Beşinci eleman 3<7, bir alta indik 3<5 olduğu için bir alta indik, 3>1 olduğu için 1'in sağına yazılır.
6. Altıncı eleman 6<7 olduğu için bir alta indik, 6>5 olduğu için 5'in sağına yazılır.
7. Yedinci eleman 0<7, 0<5, 0<1 olduğu için 1'in soluna yazılır. 
8. Sekizinci eleman 9>7 olduğu için 7'nin sağına baktık, 9>8 olduğu için 8'in sağına yazılır.
9. Dokuzuncu eleman 4<7, 4<5, 4>1 (büyük olduğu için 1'in sağını kontrol ediyoruz), 4>3 olduğu için 3'ün sağına yazılır.
10. Onuncu eleman 2<7, 2<5, 2>1, 1'in sağına 3'ü yerleştirmiştik. 2<3 olduğu için 3'ün soluna yazılır.
Şema ile gösterecek olursak:

                        7
                       / \
                      5   8
                     / \   \
                    1   6   9
                   / \
                  0   3
                     / \
                    2   4