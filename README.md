# Fizik_hesap_makinesi
Fizikçilerin kullanabileceği bir hesap makinesi
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fizik Hesap Makinesi</title>
    <!-- CSS Dosyamızı Bağlıyoruz -->
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="konteynir">
        <h1>Fizik Hesaplayıcı</h1>
        <div class="kart">
            <h3>1. Fizik Dalı Seçin</h3>
            <select id="kategori" onchange="formulleriGuncelle()">
                <option value="">-- Alan Seçiniz --</option>
                <option value="mekanik">Mekanik</option>
                <option value="termo">Termodinamik</option>
                <option value="elektrik">Elektromanyetizma</option>
                <option value="modern">Modern Fizik</option>
                <option value="optik">Optik</option>
                <option value="donusturucu">Dönüştürücü</option>
            </select>
            <div id="formul-alani" style="display:none;">
                <h3>2. İşlem Seçin</h3>
                <select id="formul" onchange="inputlariHazirla()"></select>
            </div>
        </div>

        <div id="input-karti" class="kart" style="display:none;">
            <h3 id="formul-baslik">Verileri Giriniz</h3>
            <div id="inputlar"></div>
            <button onclick="hesapla()">HESAPLA</button>
            <div id="sonuc-ekrani" class="sonuc-kutusu"></div>
            <div id="hata-ekrani" class="hata-kutusu"></div>
        </div>
    </div>
    <!-- JS Dosyamızı Bağlıyoruz -->
    <script src="script.js"></script>
</body>
</html>
