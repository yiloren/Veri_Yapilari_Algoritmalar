# **2. MERGE SORT PROJESİ**
---
[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
---


## **1. Merge Sort**


```
Dizinin merge sort türüne göre adımları:
1.                          [16,21,11] [8,12,22]
2.                       [16] [21,11]   [8,12] [22]
3.                       [16] [11,21]   [8,12] [22]
4.                          [11,16,21] [8,12,22]
5.                           [8,11,12,16,21,22]
```

## **Aşamalar şu şekilde olacaktır:**
### ***1.1 Aşama***
Sıralı olmayan diziyi ortadan eşit olarak iki alt diziye ayırır
```
[16,21,11] ile [8,12,22]
```

### ***1.2. Aşama***
Bu ayırma işlemi, alt diziler en çok iki elemanlı olana kadar devam eder.
``` 
Sol tarafta [16] ile [21,11] 
Sağ tarafta [8,12] [22]
```
### ***1.3. Aşama***
Alt dizileri kendi içinde sıralar.
``` 
Sol tarafta [16] ile [11,21] 
Sağ tarafta [8,12] [22]
``` 

### ***1.4. Aşama***
Sıralı iki alt diziyi tek bir sıralı dizi olacak şekilde birleştirir.
``` 
Sol tarafta [11,16,21]
Sağ tarafta [8,12,22]
``` 

### ***1.5. Aşama***
İkiye ayrılmış olan dizi sıranarak birleştirilir
```
[8,11,12,16,21,22]
``` 

## **2. Big-O Gösterimi**
O(n.logn)

---
[Patika.dev](http://Patika.dev) ekibine teşekkürler.
## **![ ](https://github.com/yiloren/kodluyoruzilkrepo/blob/master/img/Twitter_icon_small.png) [yiloren](https://twitter.com/ytanidir)** 