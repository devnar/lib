# Bilgi
[CSS](#css)
1. [Renkler](#renkler)
2. [Konteyner](#container)
3. [Panel](#panel)
4. [Sınır (border)](#border)
5. [Kartlar](#cards)
6. [Yazı tipleri](#fonts)
7. [Yazı](#text)
8. [Yuvarlatma](#round)

[JS](#javascript)
1. [Seçiciler](#selectors)
2. [Gizle](#hide)
2. [Göster](#show)
3. [Stil ekle](#add-style)
4. [Sınıf ekle](#add-class)
5. [Filtreleme](#filtreleme)
6. [Sıralama](#sort)
7. [Slayt gösterim](#slide-shows)
8. [HTML içeriği](#html-includes)
9. [HTML Verilerini Görüntüle](#display-html-data)

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

#### tema
NAR'ın renk teması:
```css
.w3-theme-l5 {color:#000 !important; background-color:#f0fcfc !important}
.w3-theme-l4 {color:#000 !important; background-color:#cdf6f6 !important}
.w3-theme-l3 {color:#000 !important; background-color:#9cecec !important}
.w3-theme-l2 {color:#000 !important; background-color:#6ae3e3 !important}
.w3-theme-l1 {color:#000 !important; background-color:#38d9d9 !important}
.w3-theme-d1 {color:#fff !important; background-color:#1fa2a2 !important}
.w3-theme-d2 {color:#fff !important; background-color:#1b9090 !important}
.w3-theme-d3 {color:#fff !important; background-color:#187e7e !important}
.w3-theme-d4 {color:#fff !important; background-color:#156c6c !important}
.w3-theme-d5 {color:#fff !important; background-color:#115a5a !important}

.w3-theme-light {color:#000 !important; background-color:#f0fcfc !important}
.w3-theme-dark {color:#fff !important; background-color:#115a5a !important}
.w3-theme-action {color:#fff !important; background-color:#115a5a !important}

.w3-theme {color:#fff !important; background-color:#23b5b5 !important}
.w3-text-theme {color:#23b5b5 !important}
.w3-border-theme {border-color:#23b5b5 !important}

.w3-hover-theme:hover {color:#fff !important; background-color:#23b5b5 !important}
.w3-hover-text-theme:hover {color:#23b5b5 !important}
.w3-hover-border-theme:hover {border-color:#23b5b5 !important}
```
`<style></style>` etiketleri arasına `<head>` kısmına ekleyin

### container
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

### border
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
| nj-bottombar          | Bir öğeye kalın bir alt kenarlık ekler |
| nj-leftbar            | Bir öğeye kalın bir sol kenarlık ekler |
| nj-rightbar           | Bir öğeye kalın bir sağ kenarlık ekler |
| nj-topbar             | Bir öğeye kalın bir üst kenarlık ekler |

`nc-round-(size)` ile Yuvarlatılmış kenarlıklar eklenebilir

### cards
| Class            | Açıklama    |
| -----------      | ----------- |
| nc-card          | Herhangi bir HTML içeriği için kapsayıcı ekler |
| nc-card-2        | Herhangi bir HTML içeriği için kapsayıcı (2 piksel kenarlıklı gölge) |
| nc-card-4        | Herhangi bir HTML içeriği için kapsayıcı (4 piksel kenarlıklı gölge) |

kartları renklendirmek için `nc-(color)` komudunu kullan. Farklı bölümler eklemek için `nc-container` ekleyin. 
Örnek:
```html
<div class="nc-card-4">
  <div class="nc-display-container nc-text-white">
    <img src="https://trthaberstatic.cdn.wp.trt.com.tr/resimler/1474000/istanbul-1475727_2.jpg" alt="Lights" style="width:100%">
    <div class="nc-xlarge nc-display-bottomleft nc-padding">İstanbul 8&deg; C</div>
  </div>
  <div class="nc-row">
    <div class="nc-third nc-center">
      <h3>MON</h3>
      <img src="https://img.icons8.com/color/48/sun--v2.gif"/>
    </div>
    <div class="nc-third nc-center">
      <h3>TUE</h3>
      <img src="https://img.icons8.com/color/48/partly-cloudy-rain--v2.gif"/>
    </div>
    <div class="nc-third nc-center nc-margin-bottom">
      <h3>WED</h3>
      <img src="https://img.icons8.com/color/48/storm--v2.gif"/>
    </div>
  </div>
</div>
```

### fonts
4 farklı yerleşik yazı tipi sınıfı kullanabilirsiniz. Bunlar:

| Adı              |
| -----------      |
| nc-serif         | 
| nc-sans-serif    |
| nc-cursive       |

### text
Metni hizalamak için `nc-left-align` ve `nc-right-align` sınıfları kullanılır. `nc-wide` sınıfı daha geniş bir metin belirtir. `nc-opacity` sınıfı , tüm renklerle çalışacak şekilde tasarlanmıştır, metin opaklığını değiştirir.

### round
`` sınıflar , herhangi bir HTML öğesine yuvarlatılmış köşeler ekler.
Örnek
| Class            | Açıklama    |
| -----------      | ----------- |
| w3-round         | 4 piksellik yuvarlatılmış öğe  |
| w3-round-small   | 2 piksellik yuvarlatılmış öğe  |
| w3-round-medium  | 4 piksellik yuvarlatılmış öğe  |
| w3-round-large   | 8 piksellik yuvarlatılmış öğe  |
| w3-round-xlarge  | 16 piksellik yuvarlatılmış öğe |
| w3-round-xxlarge | 32 piksellik yuvarlatılmış öğe |

### margin padding
`nc-padding-(sayı)` sınıfları, herhangi bir HTML öğesine üst ve alt dolgu ekler. Boyutlandırmak için `small, large, 16, 24, 32, 48, 64` kullanmalısınız.

`nc-margin` sınıfı , bir öğenin tüm kenarlarına 16 piksellik bir kenar boşluğu ekler. `top, left, right, bottom` ekleyerek ne tarafına boşluk ekleneceğini ayarlayabilirsin.

## javascript
ön eki nj'dir. Basit yapılı ve ingilizcedir.

### selectors
HTML öğelerini seçer ve seçilen öğe(ler) üzerinde eylemler gerçekleştirir.

#### hide 
`nj.hide('p')` ile p elemanı gizler.

`nj.hide('#p')` ile p id'li elemanı gizler.

`nj.hide('.p')` ile p class'lı elemanı gizler.

#### show

`nj.show('p')` ile p elemanı gösterir.

`nj.show('#p')` ile p id'li elemanı gösterir.

`nj.show('.p')` ile p class'lı elemanı gösterir.

`nj.toggleShow('[p, #p, .p]')` ile seçili elemanı gizleme ile gösterme arasında geçiş yapar.

Daha fazla örnek

| Seçici       | Açıklama    |
| -----------  | ----------- |
| ("*")        | Belgedeki tüm öğeleri seçer |
| (this)       | Geçerli HTML öğesini seçer |
| ("p.intro")  | class="intro" ile tüm < p > öğelerini seçer |
| ("div p")    | Tüm < div > öğelerinin içindeki tüm < p > öğelerini seçer |
| ("div p:first-child") | Tüm < div > öğelerinin içindeki ilk < p > öğesini seçer |
| ("[href]")   | Bir href özniteliği ile tüm öğeleri seçer |
| ("a[target=_blank]")  | "_blank" değerine eşit bir hedef öznitelik değerine sahip tüm < a > öğelerini seçer |
| ("p:nth-child(even)") | Tüm hatta < p > öğelerini seçer |

#### add style

`nj.addStyle(selector,'property','value')` şeklinde kullanılır.
Örnek: 
```html
<button onclick="nj.addStyle('#text','background-color','red')">Add Style</button>
```
kodu ile `text` class'lı elemanı butona tıklandığında arkaplanını kırmızı yapar.

#### add class

`nj.addClass(selector,'class')` veya `nj.addClass(selector,'class1 class2 class3...')` şeklinde kullanılır. Sınıf ekler. 
Örnek:
```html
<button onclick="nj.addClass('h2','marked')">Add Style</button>
```
```html
<button onclick="nj.addClass('h2','background fontsize border')">Add Style</button>
```

+ sınıfları değiştir

`nj.toggleClass(selector,'property','class')` veya `nj.toggleClass(selector,'property','class1 class2 class3...')` şeklinde kullanılır. 
Örnek:
```html
<button onclick="nj.toggleClass('h2','class1','class2')">Add Style</button>
```
```html
<button onclick="nj.toggleClass('h2','class1','background fontsize border')">Add Style</button>
```

#### filtreleme

`nj.filterHTML(selector)` şeklinde kullanılır. Filtreleme yapar.
Örnek: 
```html
<input oninput="nj.filterHTML('#id01', 'li', this.value)" placeholder="Search for names..">

<ul id="id01">
  <li>Alfreds Futterkiste</li>
  <li>Berglunds snabbköp</li>
  <li>Centro comercial Moctezuma</li>
  <li>Ernst Handel</li>
  <li>FISSA Fabrica Inter. Salchichas S.A.</li>
</ul>
```

#### sort
`nj.sortHTML(selector)` şeklinde kullanılır. Sıralama yapar. 
Örnek: 
```html
<button onclick="nj.sortHTML('#id01', 'li')">Sort</button>

<ul id="id01">
  <li>Oslo</li>
  <li>Stockholm</li>
  <li>Helsinki</li>
  <li>Berlin</li>
  <li>Rome</li>
  <li>Madrid</li>
</ul>
```

#### slide shows

`nj.slideshow(selector, interval (milliseconds))` şeklinde gösterilir. Slayt gösterisi yapar.
Örnek: 
```html
<img class="nature" src="img_snowtops.jpg">
<img class="nature" src="img_mountains.jpg">
<img class="nature" src="img_nature.jpg">

<script>
nj.slideshow(".nature");
</script>
```

#### html includes

`nj.includeHTML()` şeklinde gösterilir. Bir sayfanın HTML içeriğini alır.
Örnek:
```html
<div nj-include-HTML="h1.html"></div>
<div nj-include-HTML="content.html"></div>

<script>
nj.includeHTML();
</script>
```

#### display html data
`nj.displayObject(selector)` şeklinde gösterilir. Verilerinize yer ayırmak için herhangi bir HTML öğesine {{ }} parantezleri eklemeniz yeterlidir.
Örnek:
```html
<script>
var myObject = {"firstName" : "John", "lastName" : "Doe"};
nj.displayObject("id01", myObject);
</script>
```
