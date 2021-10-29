# Asal Sayı Bulma
Girilen bir sayının asal olup olmadığını bulan uygulama

Çalışmamızda öncelikle bir algoritma akış şeması hazırladık.


![AsalSayiAkisSemasi](https://user-images.githubusercontent.com/93383609/139434632-60116f5f-8fc4-4589-9f09-044c9e982706.png)

Daha sonra yazılımı gelştireceğimiz programlama dilini seçmek için çalışmaya başladık.,
Elimizdeki seçenekler Python, Java, Html/JavaScript.
Python'da kullanıcı girişi güzel olmadığı için Java'yı düşündük. Fakat sunum yapmak istediğimiz yerde çalıştırma ortamı bulamama ihtimali olduğu için basit olan ve her tarayıcıda çalışabildiği için Html/JavaScript'e karar verdik.

  <script>
        function hesapla() {
            var sayi = document.getElementById("girilenSayi").value;
            for (sayac = 2; sayac < sayi; sayac = sayac + 1) {
                if (Number.isInteger(sayi / sayac)) {
                    alert("asal değil");
                    return;
                }
            }
            alert("asal sayı");
        }

    </script>
    <h1>Sayınız Asal Mı?</h1>
    <p>Lütfen sayınızı giriniz</p>
    <input id="girilenSayi" /> <input type="button" onclick="hesapla()" value="Sayımız Asal Mı?">
