# platform-web Yol Haritası

Fazlar [ana yol haritası](https://github.com/Libre-University/docs/blob/main/ROADMAP.md) ile hizalıdır. Akışlar: [UML.md](https://github.com/Libre-University/docs/blob/main/UML.md).

## Faz 0: İskelet (davet öncesi)

- [ ] Vite + React + TypeScript projesi, ESLint, Prettier
- [ ] CI: lint, typecheck, unit test, build, axe ile erişilebilirlik kontrolü
- [ ] OpenAPI'den istemci üretim betiği
- [ ] i18n altyapısı (tr varsayılan, en)
- [ ] Uygulama kabuğu: üst menü, yan menü, rol bazlı yönlendirme

## Faz 1: Çekirdek Platform

- [ ] OIDC ile giriş/çıkış (Authorization Code + PKCE)
- [ ] Profil sayfası
- [ ] Yönetim paneli: kullanıcı, rol, birim, dönem, ders kataloğu
- [ ] Audit log görüntüleme (yetkili denetim rolü)
- [ ] Hata, boş durum ve yükleniyor bileşenleri

## Faz 2: Akademik İş Akışları

- [ ] Öğrenci: ders seçme ekranı, çakışma ve kontenjan geri bildirimi
- [ ] Danışman: onay bekleyen kayıtlar listesi
- [ ] Akademisyen: şube listesi, not girişi tablosu
- [ ] Öğrenci: not görüntüleme, transkript taslağı indirme
- [ ] Playwright ile uçtan uca senaryolar (ders kayıt, onay, not girişi)

## Faz 3: LMS ve Self-Servis

- [ ] Ders sayfası, haftalık izlence, materyaller, duyurular
- [ ] Ödev teslimi
- [ ] Gömülü Jitsi canlı ders (IFrame API)
- [ ] Bildirim merkezi, rol bazlı ana sayfa

## Faz 4+

- [ ] Destek masası, belge talebi, ödeme durumu ekranları
