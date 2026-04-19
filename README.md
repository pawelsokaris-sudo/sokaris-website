# sokaris.pl — Strona firmowa Sokaris Oprogramowanie

Oficjalna strona firmy **Sokaris Oprogramowanie** — twórców programów **Faktura-NT** i **Sapio**.

🌐 **https://sokaris.pl**

## Stack technologiczny

- **Astro** — statyczne SSG, zero JS na kliencie (poza scroll animations)
- **LiteSpeed** — hosting Cyber_Folks
- **Inter** — Google Fonts
- **Umami** — self-hosted analytics (analytics.sokaris.pl)

## Struktura

```
src/
├── layouts/
│   └── Base.astro          # Layout z header, footer, CSS
├── pages/
│   ├── index.astro         # Strona główna (Hero, Produkty, Serwis, R&D, Kontakt)
│   └── polityka-prywatnosci.astro
public/
├── images/
│   ├── sokaris-logo.png    # Logo firmowe
│   ├── hero.png            # Hero section image
│   ├── faktura-nt.png      # Mockup Faktura-NT
│   ├── sapio.png           # Mockup Sapio ERP
│   └── support.png         # Support team photo
└── favicon.svg
```

## Sekcje strony

| Sekcja | Opis |
|--------|------|
| 🏠 Hero | "Fakturowanie, księgowość, rozwój" + CTA |
| 📊 Produkty | Faktura-NT + Sapio z mockupami |
| 🛡️ Serwis | BOK + AI Agent + Zgłoszenia + Infolinia 22 38 956 38 (Pon-Pt 9-15) |
| 🔬 R&D | ActProof.io + ActProof-OS + AioP Protocol |
| 📬 Kontakt | biuro@sokaris.pl + telefon |

## Dane firmowe

- **Sokaris Oprogramowanie** · Paweł Guzik
- ul. Błękitna 3, 46-300 Olesno
- NIP: 576-105-16-34
- Tel: 22 38 956 38
- E-mail: biuro@sokaris.pl

## Deploy

```bash
npm install
npm run build        # → ./dist/
# Upload dist/* do public_html na Cyber_Folks
```

## Rollback do WordPress

```bash
# Na Cyber_Folks SSH (port 222):
cd ~/domains/sokaris.pl
rm -rf public_html
mv public_html_wp_backup public_html
```

## Historia

- **2026-04-19**: Migracja z WordPress na Astro, jasny theme, logo, zdjęcia
- **1996–2025**: WordPress (backup w `public_html_wp_backup/`)
