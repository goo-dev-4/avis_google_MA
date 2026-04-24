# شراء تقييمات جوجل — ichtari-taqyimat.com

موقع ستاتيك بالدارجة المغربية (RTL) لخدمة شراء تقييمات جوجل فالمغرب.

- **Domain:** https://ichtari-taqyimat.com
- **Langue:** Arabe marocain (Darija) — `lang="ar"` / `dir="rtl"`
- **Devise:** MAD (درهم مغربي)
- **Hébergement:** GitHub Pages (voir [CNAME](CNAME))

## Structure

Site statique HTML/CSS pur — pas de build, pas de framework.

```
index.html                              Page d'accueil
styles.css                              Feuille de style unique
sitemap.xml                             26 URLs
robots.txt
CNAME                                   ichtari-taqyimat.com

# Pages services (8)
chira-taqyimat-salbia-google.html       شراء تقييمات سلبية
hadhf-taqyimat-google.html              حذف تقييمات جوجل
ichtari-taqyimat-google-ijabia.html     تقييمات إيجابية
ichtari-taqyimat-google-my-business.html
ichtari-taqyimat-google-5-noujoum.html  تقييم 5 نجوم
taqyimat-google-wahmia.html             تقييمات وهمية
taaziz-taqyimat-google.html             تعزيز التقييمات
tahsin-taqyim-google.html               تحسين التقييم

# Pages type d'achat (4)
chira-taqyimat-google-rakhisa.html      رخيصة
chira-taqyimat-google-charika.html      شركة
chira-taqyimat-google-haqiqia.html      حقيقية
chira-taqyimat-google-mawthouqa.html    موثوقة

# Pages métiers (13)
chira-taqyimat-google-mataam.html           مطعم
chira-taqyimat-google-foundouq.html         فندق
chira-taqyimat-google-sabbak.html           سباك
chira-taqyimat-google-tabib.html            طبيب
chira-taqyimat-google-tabib-asnan.html      طبيب أسنان
chira-taqyimat-google-mouhami.html          محامي
chira-taqyimat-google-kahrabai.html         كهربائي
chira-taqyimat-google-hirafi.html           حرفي
chira-taqyimat-google-wikala-aqaria.html    وكالة عقارية
chira-taqyimat-google-mirab-sayarat.html    ميكانيكي
chira-taqyimat-google-mokawel-stouh.html    مقاول السطوح
chira-taqyimat-google-moqallim-achjar.html  معلم الأشجار
chira-taqyimat-google-mounassiq-hadaiq.html منسق الحدائق
```

## SEO

- `hreflang="ar-MA"` + `x-default` sur toutes les pages
- Schema.org JSON-LD (`Organization`, `Service`, `FAQPage`)
- Open Graph + Twitter Card
- `sitemap.xml` avec 26 URLs + balises `image:image`
- Images au format WebP + PNG

## Déploiement

Push sur `main` → GitHub Pages publie automatiquement. Le `CNAME` gère le domaine custom.

```bash
git add .
git commit -m "update"
git push origin main
```

## Commandes utiles

```bash
# Preview local (Python)
python -m http.server 8000

# Preview local (Node)
npx serve .
```

## À faire après chaque déploiement

1. Soumettre `https://ichtari-taqyimat.com/sitemap.xml` dans Google Search Console
2. Tester le rendu mobile (RTL) sur les 26 pages
3. Vérifier les liens canoniques et hreflang
