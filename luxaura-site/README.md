# LuxAura svetainė – Netlify CMS

## Kaip paleisti

### 1. GitHub
- Sukurkite naują GitHub repozitoriją (pvz. `luxaura-site`)
- Įkelkite visus šiuos failus į ją

### 2. Netlify
- Eikite į https://netlify.com ir prisijunkite
- Spustelėkite „Add new site" → „Import an existing project"
- Pasirinkite savo GitHub repozitoriją
- Build settings palikite tuščius (statinis HTML)
- Spustelėkite „Deploy site"

### 3. Įjunkite Netlify Identity
- Savo Netlify projekte: **Site settings → Identity → Enable Identity**
- Žemiau: **Git Gateway → Enable Git Gateway**
- Pakvieskite save: **Identity → Invite users** (įveskite savo el. paštą)

### 4. Prisijunkite prie CMS
- Eikite į `https://jūsų-svetainė.netlify.app/admin/`
- Priimkite pakvietimą iš el. pašto ir nustatykite slaptažodį
- Prisijunkite ir redaguokite turinį!

## Kaip keisti turinį
1. Eikite į `/admin/`
2. Pasirinkite skyrių (pvz. "Galerija")
3. Įkelkite nuotraukas arba keiskite tekstus
4. Spustelėkite „Publish" – pakeitimai atsiranda automatiškai

## Failų struktūra
```
luxaura-site/
├── index.html          ← Pagrindinė svetainė
├── netlify.toml        ← Netlify konfigūracija
├── admin/
│   ├── index.html      ← CMS prisijungimo puslapis
│   └── config.yml      ← CMS laukų konfigūracija
├── data/               ← Redaguojamas turinys (JSON)
│   ├── hero.json
│   ├── stats.json
│   ├── about.json
│   ├── gallery.json
│   ├── services.json
│   ├── whyus.json
│   ├── contact.json
│   └── footer.json
└── images/
    ├── logo.png        ← Logotipas
    └── uploads/        ← CMS įkeltos nuotraukos
```
