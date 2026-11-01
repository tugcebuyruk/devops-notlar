---
tags: [komut, linux]
---
# Linux Komutları

## Dosya ve dizin
| Komut | Ne yapar |
|---|---|
| `pwd` | Bulunduğun dizini gösterir |
| `ls -la` | Gizli dosyalar dahil ayrıntılı liste |
| `cd /yol` | Dizin değiştirir |
| `mkdir -p a/b` | İç içe dizin oluşturur |
| `cp -r kaynak hedef` | Kopyalar |
| `mv eski yeni` | Taşır / yeniden adlandırır |
| `rm -r dizin` | Siler (dikkat!) |
| `cat dosya` | Dosyayı gösterir |

## İzinler
| Komut | Ne yapar |
|---|---|
| `chmod 755 dosya` | İzinleri değiştirir |
| `chown kullanici:grup dosya` | Sahibini değiştirir |
| `sudo komut` | Yönetici olarak çalıştırır |

## Süreç ve servis
| Komut | Ne yapar |
|---|---|
| `ps aux` | Çalışan süreçler |
| `systemctl status nginx` | Servis durumu |
| `journalctl -u nginx` | Servis logları |

Konu notu: [[Linux]]
