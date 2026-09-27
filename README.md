# platform-web

LibreUniversity web arayüzü: öğrenci, akademisyen, danışman, idari kullanıcı ve sistem yöneticisi ekranları.

## Teknoloji

- React + TypeScript, Vite
- TanStack Query, React Router
- `platform-api` OpenAPI şemasından üretilen tipli istemci (`openapi-typescript`)
- `@libre-university/ui` bileşen kütüphanesi (`design-system`)
- i18next (tr, en)
- Vitest, Testing Library, Playwright, axe-core

## İlkeler

- WCAG 2.1 AA erişilebilirlik hedefi
- Önce mobil uyumlu (responsive) tasarım
- Yetki kontrolü sunucuda yapılır; arayüz yalnızca görünürlüğü düzenler
- Harici CDN, analitik veya font servisine bağımlılık yoktur (self-hosted)

## Fazlara Göre İşler

| Faz | Bu repoda yapılacaklar |
| --- | --- |
| Faz 0 | Vite + React + TS iskeleti, CI, OpenAPI istemci üretimi, i18n, uygulama kabuğu |
| Faz 1 | OIDC girişi, profil, yönetim paneli (kullanıcı, rol, birim, dönem, ders), audit log görüntüleme |
| Faz 2 | Ders seçme, danışman onayı, not girişi, not ve transkript görüntüleme, uçtan uca testler |
| Faz 3 | Ders sayfası, materyal, ödev teslimi, gömülü Jitsi, bildirim merkezi, rol bazlı ana sayfa |
| Faz 4+ | Destek masası, belge talebi, ödeme durumu ekranları |

Ayrıntılı ve işaretlenebilir liste: [ROADMAP.md](ROADMAP.md). Fazlar [ana yol haritası](https://github.com/Libre-University/docs/blob/main/ROADMAP.md) ile hizalıdır. Açık işler için `phase:*` etiketlerine bakın.

## Katkı

Katkı rehberi, davranış kuralları ve güvenlik politikası organizasyon genelinde [`.github`](https://github.com/Libre-University/.github) reposundadır. Mimari kararlar [`docs`](https://github.com/Libre-University/docs) reposundaki ADR'lerle alınır.

## Lisans

Bu proje [GNU Affero Genel Kamu Lisansı v3.0 veya sonrası](LICENSE) (AGPL-3.0-or-later) ile lisanslanmıştır. Ağ üzerinden hizmet olarak sunulan değiştirilmiş sürümlerin kaynak kodu da kullanıcılarla paylaşılmalıdır ([ADR-0002](https://github.com/Libre-University/docs/blob/main/docs/adr/0002-prefer-agpl-3-or-later-license.md)).
