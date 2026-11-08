# WINOrganizer - PWA -> APK pres PWABuilder (bez instalace)

## Co je v balicku
- index.html - cela webova aplikace
- manifest.json - nazev, ikony, barvy, standalone rezim
- sw.js - service worker, offline cache
- icon-192.png, icon-512.png

## Krok 1 - Dej web na internet (zdarma, 2 minuty)
Varianta A - Netlify Drop:
1. Jdi na app.netlify.com/drop
2. Pretahni tam SLOZKU winorganizer-pwa (ne ZIP)
3. Dostanes adresu jako https://neco-jmeno.netlify.app

Varianta B - GitHub Pages:
1. Novy repozitar, nahraj obsah slozky winorganizer-pwa
2. Settings > Pages > Deploy from branch main
3. Adresa bude https://tvuj-ucet.github.io/nazev-repozitare/

## Krok 2 - PWABuilder
1. Jdi na https://www.pwabuilder.com
2. Vloz adresu sveho webu (musi byt https://)
3. Pockej na analyzu, klikni Build / Package
4. Vyber Android
5. Stahni .apk / .aab

## Krok 3 - Instalace do telefonu
- APK: nahraj do telefonu, povol instalaci z neznamych zdroju, nainstaluj
- AAB: pro Google Play

## Dulezite
- Web MUSI byt na https, jinak PWABuilder nepusti dale
- Puvodni aplikace uklada data jen v pameti stranky - pred zavrenim pouzij Zaloha JSON (export), po otevreni import
- Pocasi a mapove dlazdice potrebuji internet, zbytek funguje offline diky service workeru
