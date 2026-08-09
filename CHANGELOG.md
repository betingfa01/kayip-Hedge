# Changelog

## v1 — Hedge Hesaplayıcı
- Eski sabit formül ("Bahis Tutarı − Bonusun Yarısı") kaldırıldı.
- Yeni formül: Borsa Lay Tutarı = Site Stake × (Site Oranı − Bonus%) / Borsa Lay Oranı
- Site Oranı ve Borsa Lay Oranı artık zorunlu girdi — hesap artık oranları hesaba katıyor.
- Her iki sonuç senaryosu (Site kazanır / Site kaybeder + bonus) ayrı gösteriliyor, net kâr/zarar hesaplanıyor.
- Eşik oran göstergesi eklendi: mevcut borsa lay oranı, "garanti kâr" sınırının altında mı üstünde mi anında görülüyor.
- "Back" terimi Site, "Lay" terimi Borsa Lay olarak yeniden adlandırıldı.
- Görsel kimlik (renk paleti, font, kart/buton stilleri) korunarak genişletildi.
