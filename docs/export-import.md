[![GitHub license](https://img.shields.io/github/license/iqlal/migrate-to-azure)](https://github.com/iqlal/migrate-to-azure/blob/main/LICENSE)

# Dokumentasi Migrasi ke Azure Menggunakan Export-Import VM
Pada dokumentasi ini, akan diuraikan bagaimana cara migrasi VM menggunakan cara Export-Import ke Azure. Diasumsikan sudah memiliki VM yang akan di-Export dan juga Azure Subsciption yang aktif.

## Prasyarat
Pada bagian ini, pastikan semua sudah tersedia agar tidak ada kendala pada tahap berikutnya <br>
✅ Azure Subscription yang aktif <br>
✅ Virtualisasi Platform, dapat menggunakan VMware Workstation, WMware vSphere, maupun Hyper-V <br>
✅ VM yang akan di Export <br>

## Proses Export VM
Pada bagian Proses Export VM, akan dirincikan bagaimana cara Export VM pada 2 Platform (VMware & Hyper-V)

### Export VM VMware
### Export VM Hyper-V
Pada Hyper-V Manager, pilih VM yang akan di-export. Pada contoh, kami menggunakan Debian 11 CLI Edition yang terdapat Web Server Nginx untuk percobaan kemudian saat berhasil di-import ke Azure.
Klik kanan untuk membuka context menu, pilih pada bagian Export. <br>
![Hyper-V Manager](/image/export-import/1.png) <br>
Tentukan dimana letak file Export akan dibuat. <br>
![Export Location](/image/export-import/2.png) <br>
Buka letak lokasi file export VM, lalu pilih pada folder Virtual Hard Disks. Pada lokasi tersebut terdapat file yang ber-ekstensi .vhdx <br>
![VHDX](/image/export-import/3.png) <br>
Jika sudah ditemukan file tersebut, maka proses Export sudah selesai.