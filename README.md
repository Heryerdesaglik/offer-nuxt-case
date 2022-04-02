# offer-nuxt-case

Kullanıcının istediği ürünü seçip(yalnızca 1 adet ürün) bu ürün ile ilgili teklif alabileceği ve geçmiş tekliflerini görebileceği bir arayüz yapılması isteniyor.

## Teklif İsteme Aşaması
![case-1](https://user-images.githubusercontent.com/37562936/161384072-d748fcac-1cdd-4a6e-9f4b-955c7b8dc7eb.png)

Kullanıcıya sistemdeki ürünler yukarıdaki tasarımdaki gibi gösterilecek. İlgili ürünleri okumak için <code>"products.json"</code> dosyası kullanılacak. Bu dosya içerisindeki ürünler okunup tasarımdaki yerine yerleştirilecek. Bu işlem yapılırken <code>products</code>'ın <code>sequence</code> özelliğine göre sıralama yapılıp, kartlar bu sıraya göre kullanıcıya gösterilecek. Kullanıcı aynı anda tüm ürünleri göremeyeceği için ürünlerin gösterileceği component y ekseninde scrollable olmalı.

Kullanıcı ürünü seçtiğinde ilgili kartın rengi değişecek ve kartın sağ üstünde tik simgesi gözükecek.

Ürün seçiminden sonra kullanıcı mail adresini ve teklifle ilgili not girerek "Teklif İste" butonuna basacak.

<blockquote>
Not: Ürün seçilmeden, mail adresi doğru bir şekilde doldurulmadan kullanıcı teklif alamayacak. Dolayısıyla "Teklif İste" butonuna tıkladığında kullanıcıya ilgili alanlar için uyarı verilecek.
</blockquote>

## Teklif İsteme Aşamasının Tamamlanması
![case-2](https://user-images.githubusercontent.com/37562936/161384417-0a8cb5ca-4dd3-4abf-ae28-d9030e05f3f5.png)

Kullanıcı "Teklif İste" butonuna bastığında gerekli tüm alanlar doldurulmuş ise kullanıcıya yukarıdaki tasarımdaki gibi popup gösterilecek.

## Teklifleri Görüntüleme
![case-3](https://user-images.githubusercontent.com/37562936/161384456-fe5b2254-0b91-4530-8da8-c1a9695c3e6d.png)

Kullanıcı tekliflerini istediği zaman "Teklifleri Görüntüle" butonuna bastığında görüntüleyebilecek. Burada görüntülenecek teklifler <code>"offers.json"</code> dosyası içerisindeki teklifler olacak. Görüntülenecek tekliflerin sıralaması, en yakın tarihli teklif en üstte yer alacak şekilde tarihe göre olacak.

Tekliflerin görüntüleneceği kartlar ilk örnekteki gibi(Midi Doğum Paketi - Beklemede) kapalı(collapse) bir şekilde yer alacak. Kullanıcı karta tıkladığında kart aşağıya doğru açılacak ve 2. örnekteki(Midi Doğum Paketi - Onaylandı) gibi gözükecek.

## Mobil
Yapılan bu tasarımlar kendi yorumunuza göre mobil cihazlar için de uyarlanmalı. Bu kısımda esnek davranabilirsiniz ancak önemli olanın kullanıcı deneyimi olduğunu unutmayalım.
