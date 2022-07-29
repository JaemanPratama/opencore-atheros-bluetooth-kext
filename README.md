# opencore-atheros-kext

Saya telah menguji ini pada macOS 10.14.6 - 11.6.8 dengan kartu kombo Wifi/BT AR9565. Kexts telah dikembangkan oleh pengembang  [itlwm zxystd](https://github.com/zxystd) 
 
Latar Belakang:
Metode terakhir yang berhasil untuk mengunggah firmware adaptor Bluetooth Atheros 3012 saat start dingin di Hackintosh adalah kext sumber tertutup yang dikembangkan oleh @EMlyDinEsH yang tidak akan berfungsi di luar macOS 10.12. Pada bulan September 2020, zxystd merilis kexts Ath3kBT dan Ath3kBTInjector untuk mengunggah firmware dan memasukkan id untuk mengaktifkan sakelar Nyala/Mati di Bluetooth PrefPane untuk chip AR3012 di macOS 10.15+. Kexts baru-baru ini ditingkatkan untuk kompatibilitas dengan macOS 10.12+. 

<img src="https://github.com/JaemanPratama/opencore-atheros-bluetooth-kext/blob/master/Image/Bluetooth%202.jpg">

:warning: Peringatan: Ath3kBTInjector : 

️kext memiliki cacat kecil: jika Anda ingin mengaktifkan / menonaktifkan Bluetooth , Anda harus mematikan Wi-Fi terlebih dahulu.  
Ath3kBTInjector dapat dihindari bagi mereka yang tidak keberatan tombol On/off bluetooth berwarna abu - abu di Bluetooth PrefPane.

Unduh :
[Halaman Github](https://github.com/zxystd/AthBluetoothFirmware/releases)

Tutorial :
1. Unduh versi terbaru dari repo Github pengembang. 
2. Tempatkan Ath3kBT.kext dan Ath3kBTInjector.kext di folder OpenCore kexts Anda. 
3. Di OpenCore Config.plist, tambahkan dua kext di bawah Kernel->Tambahkan kext lainnya dan aktifkan. Simpan konfigurasi Anda yang telah dimodifikasi setelahnya. 
4. Reboot Hackintosh Anda.

️:warning: Peringatan : \
Perhatikan bahwa, di OpenCore Ath3kBTInjector harus dimuat setelah Ath3kBT. 

<details>
<summary>Informasi Bluetooth</summary>
<img src="https://github.com/JaemanPratama/opencore-atheros-bluetooth-kext/blob/master/Image/Bluetooth%201.jpg">
</details>


Sumber: \
https://github.com/zxystd/AthBluetoothFirmware

Kredit: \
[zxystd](https://github.com/zxystd)
