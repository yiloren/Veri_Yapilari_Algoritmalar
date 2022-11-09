# **1. INSERTION SORT PROJESI**
---
[22,27,16,2,18,6] -> Insertion Sort

## 1.0. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

## Big-O gösterimini yazınız.

## 1.1. Average case: Aradığımız sayının ortada olması.
## 1.2. Worst case: Aradığımız sayının sonda olması.
## 1.3. Best case: Aradığımız sayının dizinin en başında olması.
## 1.4. Time Complexity: Dizi sıralandıktan sonra 18 sayısı yukarıdaki case'lerden hangisinin kapsamına girer? Yazınız.
---
#

## **1.0 Insertion Sort**


```
Dizinin merge sort türüne göre adımları:
1.                       [22,27,16,2,18,6]
2.                       [16,22,27,2,18,6]
3.                       [2,16,22,27,18,6]
4.                       [2,16,18,22,27,6]
5.                       [2,6,16,18,22,27]
```

## **Aşamalar şu şekilde olacaktır:**
### ***1.0.1 Aşama***
Dizinin 1. elemanı sağındaki 2. eleman ile kıyaslanır. 
22<27 olduğu için sıralama aynı kalır.
```
[22,27,16,2,18,6]
```

### ***1.0.2. Aşama***
Dizinin 2. elemanı sağındaki 3. eleman ile kıyaslanır. 
16<27 olduğu için 3. eleman ve 2. elemanın önüne gelir.
``` 
[22,16,27,2,18,6]
```
Dizinin sıralamada yeni 2. elemanı solundaki 1. eleman ile kıyaslanır.
16<22 olduğu için yeni 2. eleman 1. elemanın önüne gelir.
``` 
[16,22,27,2,18,6]
``` 
### ***1.0.3. Aşama***
Dizinin 3. elemanı sağındaki 4. eleman ile kıyaslanır
2<27 olduğu için 4. eleman 3. elemanın önüne gelir
``` 
[16,22,2,27,18,6]
``` 
Dizinin yeni 3. elemanı solundaki 2. eleman ile kıyaslanır
2<22 olduğu için 3. eleman 2. elemanın önüne gelir
``` 
[16,2,22,27,18,6]
``` 
Dizinin yeni 2. elemanı solundak 1. eleman ile kıyaslanır
2<16 olduğu için 2. eleman 1. elemanın önüne gelir
``` 
[2,16,22,27,18,6]
``` 

### ***1.0.4. Aşama***
Dizinin 4. elemanı sağındaki 5. eleman ile kıyaslanır
18<27 olduğu için 5. eleman 4. elemanın önüne gelir
``` 
[2,16,22,18,27,6]
``` 
Dizinin yeni 4. elemanı solundaki 3. eleman ile kıyaslanır
18<27 olduğu için 4. eleman 3. elemanın önüne gelir
``` 
[2,16,18,22,27,6]
``` 
### ***1.0.5. Aşama***
Dizinin 5. elemanı sağındaki 6. eleman ile kıyaslanır
6<27 olduğu için 6. eleman 5. elemanın önüne gelir
``` 
[2,16,22,18,6,27]
``` 
Dizinin yeni 5. elemanı solundaki 4. eleman ile kıyaslanır
18<27 olduğu için 5. eleman 4. elemanın önüne gelir
``` 
[2,16,18,6,22,27]
``` 
Dizinin yeni 4. elemanı solundaki 3. eleman ile kıyaslanır
6<18 olduğu için 4. eleman 3. elemanın önüne gelir
``` 
[2,16,6,18,22,27]
``` 
Dizinin yeni 3. elemanı solundaki 2. eleman ile kıyaslanır
6<16 olduğu için 3. eleman 2. elemanın önüne gelir
``` 
[2,6,16,18,22,27]
``` 
Dizinin yeni 2. elemanı solundaki 1. eleman ile kıyaslanır
2<6 olduğu için 2. eleman 2. elemanın pozisyonunda kalır.
Dizinin son elemanının ilk elemanı ile kıyaslanması bittiği için sıralanma tamamlanmıştır.
``` 
[2,6,16,18,22,27]
``` 
## **1.1. Average case: Aradığımız sayının ortada olması**
### Average case için durumu Hesaplanması n+(n-2)+(n-4)+n-6... + (n-n)--> n + ((n-1)/2)*(n-2)/2 dir --> (n^2+n+2)/4 
### Big  O notation da en büyük üstlü sayı katsayısı olmaksızın domine durumu belirleyeceği için sonucu time complexity olarak O(n^2) dir. 
Dizinimizde [6,16,22,2,18,27]
#
## **1.2. Worst case: Aradığımız sayının sonda olması**
### Worst Case durumu Hesaplanması n+(n-1)+(n-2)... +0
### Bunun toplamı da (nx(n-1))/2 dir big  O notation da en büyük üstlü sayı katsayısı olmaksızın domine durumu belirleyeceği için sonucu time complexity olarak O(n^2) dir. 
Dizinimizde [27,22,18,16,6,2]
#
## **1.3. Best case: Aradığımız sayının başta olması**
### Best Case için dizin zaten sıralıdır
### Tüm sıra sıralı olduğunundan domine durumu zaten olduğu gibidir ve time complexity olarak O(n) dir. 
Dizinimizde [2,6,16,18,22,27]
#
## **1.4. Time Complexity: Dizi sıralandıktan sonra 18 sayısı yukarıdaki case'lerden hangisinin kapsamına girer? Yazınız.**
### Sıralamanın ortasında bulunduğu için Average Case kapsamına grirer.
---
[Patika.dev](http://Patika.dev) ekibine teşekkürler.
## **![ ](https://github.com/yiloren/kodluyoruzilkrepo/blob/master/img/Twitter_icon_small.png) [yiloren](https://twitter.com/ytanidir)** 