# Archivo : provenance du fichier

| fichier | octets | sha256 | glyphes | axes | nom interne | version | copyright |
|---|---|---|---|---|---|---|---|
| Archivo-variable-latin.woff2 | 90 104 | e3a28eade21a900c7155a247757f4b2834c07bb7ef07ad7efa55cebaac1e8f5e | 302 | wght 100–900 (défaut 600), wdth 62–125 (défaut 100) | Archivo SemiBold | Version 2.001 | Copyright 2020 The Archivo Project Authors (https://github.com/Omnibus-Type/Archivo) |

Relevé le 09/10/2026 avec fontTools (tables fvar, name, maxp, GSUB). 302 glyphes : c'est le
sous-ensemble « latin » que Google Fonts sert, pas la fonte complète.

- Famille : Archivo. Créateur : Héctor Gatti (Omnibus-Type), développement Yorlmar Campos.
  Dépôt officiel : https://github.com/Omnibus-Type/Archivo. Licence : SIL Open Font License 1.1
  (OFL.txt à côté, téléchargé depuis le dépôt officiel :
  https://raw.githubusercontent.com/Omnibus-Type/Archivo/master/OFL.txt). Prix : 0 €.
- Canal : l'API css2 de Google Fonts, l'un des deux canaux que BRIEF.md autorise.
  - requête : https://fonts.googleapis.com/css2?family=Archivo:wdth,wght@62..125,100..900&display=swap
    (User-Agent Chrome 129, pour obtenir les blocs woff2) ;
  - fichier servi pour le sous-ensemble « latin » :
    https://fonts.gstatic.com/s/archivo/v25/k3kQo8UDI-1M0wlSfdnoLg.woff2 ;
  - unicode-range déclaré par Google pour ce fichier : U+0000-00FF, U+0131, U+0152-0153,
    U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+0304, U+0308, U+0329, U+2000-206F, U+20AC, U+2122,
    U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD ;
  - téléchargé le 09/10/2026 ; magic bytes wOF2 vérifiés.
- Fonte VARIABLE, un seul fichier : le skill design-as-code (fetch_fonts.py) n'accepte que des
  graisses statiques parce qu'une variable se rastérise en Type3 dans un PDF Chrome ; ce piège
  n'existe pas pour une page web, et un seul fichier de 90 Ko pèse moins que quatre statiques.
  Rôles servis : texte courant 400, lectures et timecodes 700 (chiffres tabulaires, tnum),
  titres 900 en chasse 125 %.
- Fonctions OpenType présentes : ccmp, dnom, frac, liga, locl, numr, pnum, rvrn, tnum.
- Couverture anglaise : 100 % (`couverture.py --langue en`, 09/10/2026).
- Préchargée (`<link rel="preload">`), `font-display: swap`.
