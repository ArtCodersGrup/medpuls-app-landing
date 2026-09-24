# MedPuls App — Ilova Reklama Sahifasi

MedPuls mobil ilovasi (bemorlar uchun — klinika qidirish, onlayn navbat) haqida bir sahifali (single-page) reklama/yuklab olish sahifasi.

**Jonli manzil (rejalashtirilgan):** `https://app.medpuls.uz/` (GitHub Pages, custom domain — hozircha faollashtirilmagan, quyiga qarang)

Bu sahifa `medpuls.uz` (klinikalar uchun MedPuls CRM sotuv sahifasi, boshqa repo: `MedPuls-lending`) dan farqli — bu sahifa **bemorlar** uchun, mobil ilovani tanishtirish va yuklab olishga undash uchun.

## Fayl tuzilishi

```
medpuls-app-landing/
├── index.html          # butun sahifa: HTML + CSS bitta faylda, build kerak emas
├── CNAME                # app.medpuls.uz — GitHub Pages custom domain
├── assets/
│   ├── logo.png          # MedPuls belgisi (mobil ilova repo'sidan olingan)
│   ├── screen-home.png   # ilova bosh sahifasi skrinshoti
│   ├── screen-clinic.png # klinika tafsiloti skrinshoti
│   └── screen-booking.png# yozilish oqimi skrinshoti
└── README.md
```

## Dizayn tizimi

`medpuls-app` (Flutter ilovasi) va `medpuls.uz`/`crm.medpuls.uz` bilan bir xil teal/slate palitra:

| Token | Qiymat |
|---|---|
| `teal-600` (asosiy) | `#0D9488` |
| `teal-700` (tugma foni) | `#0F766E` |
| `teal-900` (hero/footer fon) | `#0C302E` |
| Shrift | Inter (400–800) |

## Hozirgi holat

- App Store/Google Play tugmalari **"Tez orada"** holatida — do'kon akkauntlari hali ochilmagan.
- Skrinshotlar Figma dizaynidan olingan (haqiqiy ilova build'idan emas) — ilova tayyor bo'lgach yangilanishi kerak.

## Deploy (GitHub Pages)

```bash
git add -A
git commit -m "yangilanish"
git push
```

**Faollashtirish (bir martalik, qo'lda):** Repo private bo'lgani uchun GitHub Pages avtomatik yoqilmagan bo'lishi mumkin (private repo'larda Pages uchun GitHub Team/Enterprise reja kerak bo'ladi, yoki repo public qilinishi kerak). Settings → Pages → Source: `main` / `(root)` → Save. DNS'da `app.medpuls.uz` uchun CNAME yozuvi GitHub Pages'ga yo'naltirilishi kerak (`medpuls.uz` domenining DNS provayderi — aHost — orqali, `medpuls_crm/docs/infrastructure.md`ga qarang).

## Keyingi qadamlar

- [ ] Repo'ni public qilish yoki GitHub Pages uchun mos reja
- [ ] DNS: `app.medpuls.uz` → GitHub Pages
- [ ] Do'kon akkauntlari tayyor bo'lgach — haqiqiy App Store/Play Store havolalarini ulash
- [ ] Skrinshotlarni haqiqiy ilova build'idan yangilash
