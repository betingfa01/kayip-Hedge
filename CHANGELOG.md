# Changelog

## v2 — Final sürüm
- Tüm sayısal alanlar (Bahis, Site Oranı, Borsa Lay Oranı, Bonus %) `type="number"`'dan `type="text" inputmode="decimal"`'e geçirildi — bazı cihazların yerel ayarına göre virgül göstermesi sorunu tamamen giderildi.
- Yazarken canlı temizleme: virgül anında noktaya çevriliyor, sayı ve tek nokta dışındaki karakterler engelleniyor (tüm 4 alanda tutarlı).
- Oran alanlarında (Site/Borsa Lay): nokta girilmeden yazılan değerler (örn. "165") alandan çıkılınca otomatik "1.65" olarak yorumlanıyor.
- "Site Oranı" ve "Borsa Lay Oranı" etiketleri simetrik hale getirildi; back/lay ayrımı "Site back Oranı" biçiminde düz metin olarak taşındı, ayrıca giriş kutusu prefix'lerinde "@back" / "@lay" olarak gösteriliyor.
- Kullanılmayan CSS (eski rozet/badge stilleri, eşik kutusu, alt yazı, footer) temizlendi.
- JS'te tekrar eden "ondalık temizleme" mantığı tek bir `cleanDecimalInput()` fonksiyonunda birleştirildi.
- Hata durumunda eski sonuçların ekranda asılı kalması düzeltildi.

## v1 — Hedge Hesaplayıcı
- Eski sabit formül ("Bahis Tutarı − Bonusun Yarısı") kaldırıldı.
- Yeni formül: Borsa Lay Tutarı = Site Stake × (Site Oranı − Bonus%) / Borsa Lay Oranı
- Site Oranı ve Borsa Lay Oranı artık zorunlu girdi — hesap artık oranları hesaba katıyor.
- Her iki sonuç senaryosu (Site kazanır / Site kaybeder + bonus) ayrı gösteriliyor, net kâr/zarar hesaplanıyor.
- "Back" terimi Site, "Lay" terimi Borsa Lay olarak yeniden adlandırıldı.
- Görsel kimlik (renk paleti, font, kart/buton stilleri) korunarak genişletildi.
