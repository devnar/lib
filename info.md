# Bilgi
[CSS](#css)
1. [Renkler](#renkler)
2. [Konteyner](#konteyner)
3. [Panel](#panel)
4. [Sınır](#sınır-(border))

[JS](#JavaScript)
1. [Seçiciler](#seçiciler)
2. [Gizle/Göster](#gizle/göster)
3. [Stil ekle](#stil-ekle)
4. [Sınıf ekle](#sınıf-ekle)
5. [Filtreleme](#filtreme)
6. [Sıralama](#sıralama)
7. [Slayt gösterim](#slayt-gösterim)
8. [HTML içeriği](#HTML-içeriği)
9. [HTML Verilerini Görüntüle](#HTML-verilerini-görüntüle)
10. [Http istekleri](#Http-istekleri)
11. [Denetleyiciler](#denetleyiciler)
12. [Data](#data)

## CSS

### Renkler
ön eki nc'dir. Basit yapılı ve ingilizcedir. Yazıya renk verebilir.

örnek kullanım: 
```html
<div class="nc-text-cyan">Lorem ipsum dolor sit amet.</div>
```

Arkaplanınada renk verebilir.

örnek kullanım: 
```html
<div class="nc-black">Lorem ipsum dolor sit amet.</div>
```

Sınırada renk verebilirsin

örnek kullanım: 
```html
<div class="nc-border-cyan">Lorem ipsum dolor sit amet.</div>
```

Nesnenin üzerine (fare ile) geldiğinde renk değiştirebilir.

örnek kullanım: 
```html
<div class="nc-black nc-hover-cyan">Lorem ipsum dolor sit amet.</div>
```
örnek kullanım: 
```html
<div class="nc-text-black nc-hover-text-cyan">Lorem ipsum dolor sit amet.</div>
```
Renk çeşitleri:
1. Siyah (black)
2. Mavi (blue)
3. Kahverengi (brown)
4. Camgöbeği (cyan)
5. Yeşil (green)
6. Turuncu (orange)
7. Pembe (pink)
8. Mor (purple)
9. Kırmızı (red)
10. Sarı (yellow)
11. Beyaz (white)
12. Gri (grey)

### Konteyner
`nc-container` sınıfı gibi tüm HTML konteyner elemanları kullanmak için mükemmel sınıftır:


örnek kullanım: 
```html
<div class="nc-container">Lorem ipsum dolor sit amet.</div>
```

ayrıca bu koda renk ekleyebilirsin.

örnek kullanım: 
```html
<div class="nc-container nc-black">Lorem ipsum dolor sit amet.</div>
```

### panel
`nc-panel` HTML ögesine her yönden 16px dolgu ekler.

örnek kullanım: 
```html
<div class="nc-panel nc-black">Lorem ipsum dolor sit amet.</div>
```

Alıntılar içinde kullanılabilir.

örnek kullanım: 
```html
<div class="nc-panel nc-leftbar nc-sand nc-xxlarge nc-serif">Lorem ipsum dolor sit amet.</div>
```

Kart olarakta kullanılabilir.

örnek kullanım: 
```html
<div class="nc-panel nc-black nc-card-4">Lorem ipsum dolor sit amet.</div>
```

`nc-round` komutu ile kenarları yuvarlanabilir. `-small, -medium, -large, -xlarge, -xxlarge` şeklinde ne kadar yuvarlanıcağını ayarlayabilirsin.

### sınır (border)
`nc-border` aşağıdaki sınır sınıflarını sağlar:

| Syntax                | Açıklama    |
| -----------           | ----------- |
| nc-border-top         | Bir öğeye üst kenarlık ekler |
| nc-border-right       | Bir öğeye sağ kenarlık ekler |
| nc-border-left        | Bir öğeye sol kenarlık ekler |
| nc-border-bottom      | Bir öğeye alt kenarlık ekler |
| nc-border-0           | Tüm sınırları kaldırır       |
| nc-border-(color)     | Kenarlığı belirli bir renkte görüntüler |
| nc-hover-border-(color) | Üzerine gelinebilir bir kenarlık rengi ekler |
| w3-bottombar          | Bir öğeye kalın bir alt kenarlık ekler |
| w3-leftbar            | Bir öğeye kalın bir sol kenarlık ekler |
| w3-rightbar           | Bir öğeye kalın bir sağ kenarlık ekler |
| w3-topbar             | Bir öğeye kalın bir üst kenarlık ekler |

`nc-round-(size)` ile Yuvarlatılmış kenarlıklar eklenebilir

## JavaScript

### seçiciler
HTML öğelerini seçer ve seçilen öğe(ler) üzerinde eylemler gerçekleştirir.
