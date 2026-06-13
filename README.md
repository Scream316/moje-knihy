# Moje knihy - Seznam knih které chci koupit

Veřejná stránka na GitHub Pages s mým seznamem knih které si chci koupit.

## Jak to funguje

- Knihy jsou uchovány v souboru `books.json`
- Stránka načte knihy z JSONu a zobrazí je jako karty
- Každá kniha má:
  - Název
  - Autora
  - Odkaz na Dobrovského (pro proklik)
  - Obálku (buď manuálně vloženou, nebo placeholder)

## Jak přidat knihu

1. Uprav soubor `books.json` v GitHub repozitáři
2. Přidej novou knihu ve formátu:

```json
{
  "nazev": "Název knihy",
  "autor": "Autor knihy",
  "dobrovskyUrl": "https://dobrovsky.cz/product/xxx",
  "obalkaUrl": "https://example.com/cover.jpg"
}
```

3. **Povinné:** `nazev`, `autor`, `dobrovskyUrl`
4. **Nepovinné:** `obalkaUrl` (pokud ho nevyplníš, použije se placeholder)

## Nasazení na GitHub Pages

1. Vytvoř nový repozitář na GitHubu (např. `moje-knihy`)
2. Nahraj tyto soubory:
   - `index.html`
   - `books.json`
   - `README.md`
   - `cover-placeholder.jpg` (obálka placeholder, např. 300x400 px)
3. Přijdi na Settings → Pages
4. Zvol "Source: Deploy from a branch"
5. Vyber branch (např. `main`) a folder (`/ (root)`)
6. GitHub Pages bude nasazeno na: `https://TVOJE-UK.github.io/moje-knihy/`

## Sdílení

Stránka má Open Graph metadata (`og:title`, `og:description`, `og:image`), takže se při sdílení na chatu nebo sociálních sítích hezky zobrazí náhled.

---

Hostováno na [GitHub Pages](https://pages.github.com/)
