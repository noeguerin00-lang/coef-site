# Le site de Coef

Les trois pages publiques de **Coef — focus et moyennes** : présentation,
politique de confidentialité, aide et contact. Publiées par GitHub Pages sur
<https://noeguerin00-lang.github.io/coef-site/>.

Ce dépôt est **public** parce qu'Apple exige deux URL accessibles à tous
(politique de confidentialité et assistance) et que GitHub Pages est gratuit
sur un dépôt public. Le code de l'app, lui, reste dans le dépôt privé `Coef`.

## Ces pages ne s'écrivent pas ici

`confidentialite.html` est **générée** depuis la source unique de l'app
(`src/legal/confidentialite.ts` du dépôt `Coef`) : l'écran « Politique de
confidentialité » de l'app et cette page disent donc exactement la même
chose. Modifier le HTML à la main ici les ferait diverger.

Pour mettre à jour, depuis le dépôt `Coef` :

```powershell
npm.cmd run docs
copy docs\*.html ..\coef-site\
cd ..\coef-site
git add -A
git commit -m "Mise à jour des pages"
git push
```

GitHub Pages republie tout seul en une minute environ.

## Contact

<coef.app.contact@gmail.com>
