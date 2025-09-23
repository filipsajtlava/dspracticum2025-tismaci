# dspracticum2025-tismaci
Repository of group "Tismaci" for the course M7DataSP.

### 1. 
Ked poprvykrat pouzijete nejaku novu libku, prosim zapiste ju do *requirements.txt*. Vdaka tomu je mozne zadat do prikazoveho riadku nasledovne:
- pip install -r requirements.txt
Cim sa vsetky libky ktore nemate nainstaluju, a tie ktore mate sa nezmenia. Takze vlastne nemusite nic riesit. Dobre by bolo vytvorit si tzv. virtual-environment ktory sluzi na to, aby sa tie libky medzi sebou nebili s tymi, ktore uz mate nainstalovane, toto je trochu komplikovanejsie, takze ak neviete, tak zatial na to kaslite, alebo CHATGPT.


### 2.
Bolo by dobre si stiahnut git a naucit s nim pracovat ([link na stiahnute](https://git-scm.com/downloads/win)).
Treba vediet len uplne zakladne veci:
```bash
- git clone https://github.com/filipsajtlava/dspracticum2025-tismaci
```
Git vam v podstate vytvori zlozku ktora je presne taka ista ako na Githube (v podstate ju stiahne do directory v ktorej sa prave nachadzate). Robime len na zaciatku, ked prvykrat stahujeme.
```bash
- git add .
```
Po tom ako ste vykonali zmeny tymto sposobom ich urcite na commit a upload na github.
```bash
- git commit -m "popis zmien"
```
Tymto commandom commitnete svoje zmeny ktore ste oznacili pomocou add a pridate k tomu poznamku "nejaky text", zvycajne napr. zmeny ktore ste vykonali - "vytvoril som datovy subor obrazkov"
```bash
- git push
```
Tieto zmeny nasledne pushnete na internet do githubu. Pri prvom pouziti bude potrebovat zadat vas ucet, resp. repositar do ktoreho to vlastne pushujete. *POZOR! KED NIECO ZMAZEM A TIETO ZMENY BUDEM UKLADAT A NAKONIEC PUSHNEM, ZMAZEM TO PRE KAZDEHO.*
```bash
- git pull
```
Tymto si stiahnem najnovsiu verziu repozitara na Githube, takze budeme mat aktualne subory aj s upravami ostatnych.