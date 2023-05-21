# Başlangıç Seviye Java ile Backend Web Development Patikası

# Veri yapıları ve algoritmalar dersi 
---

# Merge Sort projesi 


## 1.SORUNUN CEVABI
Merge Sort'a ait Big-O notasyonu, O(nlog<sub>2</sub>n) dir.

## 2.SORUNUN CEVABI
[16, 21, 11, 8, 12, 22] dizimizi, öncelikli olarak 2'ye ayırıyoruz. Eleman sayısının çift olması bu bağlamda bir kolaylık sağlıyor.

Ortaya çıkan yeni dizilim: 
[16, 21, 11] ve [8, 12, 22]'dir. ([16, 21, 11] dizisi 1 numaralı dizi olarak adlandırılacaktır keza [8, 12, 22] diziside 2 numaralı dizi olarak adlandırılacaktır.) 

Bir sonraki aşamada 1 numaralı dizi şöyle ayrılır: [ 16 ] ve [21, 11]

2 numaralı dizinin dağılış şekli ise şöyledir: [22, 46] ve [ 7 ].

Bir sonraki adımda ise tüm sayıların 1 er adet olmak üzere ayrıldığını görüyoruz.

Tamamıyla birbirinden ayrılan sayılar, bir sonraki ana husus olan merge işlemine tabii tutulmaktadır. Merge işlemiyle, yan yana olan sayılar birleştirilirken, birleşmeden hasıl olan grup, büyüklük-küçüklük sırasına göre dizilmiş olarak peyda oluyor.

Birbirinden ayrılmış olan sayıların birleşim görünümlerini sırası ile yazıyorum:

[ 16 ] [11, 21]                            [8, 12] [ 22 ]

[11, 16, 21]                               [8, 12, 22] 

                [8, 11, 16, 21, 22]

Bu vesileyle dizimizi büyüklük-küçüklük sırasına göre dizilmiş sayılardan müteşekkil kılıyoruz.