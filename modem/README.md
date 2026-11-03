# modem.img (ingres OS2.0.8.0.ULJCNXM)

`modem.img` (281 MB) dipecah menjadi beberapa bagian < 100 MB karena batas ukuran
file GitHub. Saat build, `device/xiaomi/ingres/Android.mk` menggabungkannya kembali
menjadi `$(PRODUCT_OUT)/modem.img`, mengecek SHA1, lalu memasukkannya ke OTA
(AB_OTA_PARTITIONS `modem`).

- SHA1   : c2a132566e51ccad4cc0d423d137459de3b6ce99
- SHA256 : lihat https://github.com/kingD2N/firmware_Update/releases/tag/ingres-firmware-OS2.0.8.0.ULJCNXM

Menggabung manual: `cat modem.img.part* > modem.img`
