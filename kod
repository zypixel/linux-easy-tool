import os

def sistem_guncelle():
    os.system("sudo apt update && sudo apt upgrade -y")

def monitor_modu_ac():
    os.system("sudo airmon-ng start wlan0")

def dpkg_configure():
    os.system("sudo dpkg --configure -a")

def wifi_aglari_tara():
    os.system("sudo iwlist wlan0 scan")

def populer_araclari_yukle():
    arac_listesi = [
        "beef",
        "airgeddon",
        "wifite",
        "aircrack-ng",
        "wireshark"
    ]

    print("\nPopüler araçlar:")
    for index, arac in enumerate(arac_listesi, start=1):
        print(f"{index}. {arac}")

    secilen_arac = int(input("\nYüklemek istediğiniz aracın numarasını girin: "))

    if secilen_arac > 0 and secilen_arac <= len(arac_listesi):
        secilen_arac_adi = arac_listesi[secilen_arac - 1]
        os.system(f"sudo apt install -y {secilen_arac_adi}")
        print(f"{secilen_arac_adi} aracı başarıyla yüklendi.")
    else:
        print("Geçersiz araç numarası!")

while True:
    print("\n1. Sistem Güncelleme ve Paket Yükseltme")
    print("2. Monitor Mod Açma")
    print("3. dpkg Configure -a")
    print("4. WiFi Ağlarını Tara")
    print("5. En Popüler Araçları Yükle")
    print("6. Çıkış")

    secim = input("\nBir seçenek numarası girin: ")

    if secim == "1":
        sistem_guncelle()
    elif secim == "2":
        monitor_modu_ac()
    elif secim == "3":
        dpkg_configure()
    elif secim == "4":
        wifi_aglari_tara()
    elif secim == "5":
        populer_araclari_yukle()
    elif secim == "6":
        print("Araç kapatılıyor...")
        break
    else:
        print("Geçersiz seçenek!")

print("Araç kapatıldı.")
