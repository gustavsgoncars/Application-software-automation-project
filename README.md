# Lietojumprogrammatūras automatizēanas rīki projekta README.md
## Projekta uzdevums
Šis projekts ir izveidots ar mērķi automātiski iegūt informāciju par maršrutiem, kas jāveic no lietotāja ievadītās dzīves vietas, līdz RTU ēkām, kur norisināsies lietotāja lekcijas sekojošajā mēnesī. Šādā veidā atvieglojot ikdienas laika plānošanu. Projektā izmantotas nodarbibas.rtu.lv un Google Maps vietnes. Programma apstrādā lietotāja ievadīto informāciju, automātiski pārlūko nodarbibas.rtu.lv, iegūst lekciju informāciju, un tad izmanto Google Maps, lai aprēķinātu un iegūtu maršrutu no lietotāja norādītās izbraukšanas vietas līdz lekcijas norises vietai. Pēc tam informācija tiek apkopota Excel failā.

## Izmantotās Python bibliotēkas
- [Selenium](https://www.selenium.dev/documentation/en/): Izmantota, lai automatizētu lietotāja darbību ar tīmekļa pārlūkiem un iegūtu informāciju no nodarbibas.rtu.lv un Google Maps. 

- [openpyxl](https://openpyxl.readthedocs.io/en/stable/): Izmantota, lai izveidotu Excel failu, kurā saglabātā informācija par lekciju laikiem, norises vietām un maršrutiem.

- [unidecode](https://pypi.org/project/Unidecode/): Nodrošina iespēju stradāt ar latviešu valodā izmantotajiem burtiem.

- [re](https://docs.python.org/3/library/re.html): Izmantota adrešu apstrādei.

## Pirms programmatūras palaišanas

**Instalācijas:**
   - Tiek izmantota Selenium biblotēka, kas nestrādā GitHub Codespace vidē, tādēļ lejuplādējiet final.py, ielas.xlsx un nos.xlsx, ievietojiet to sev vēlamā mapē (folder) tālākam darbam.
   - Pārliecinieties, ka jūsu datorā ir instalēts Python.
   - Ieninstalējiet vajadzīgās biblotēkas (selenium, openpyxl, unidecode)

## Programmatūras palaišana

1. **Lietotāja ievadītie dati**
   - Sākotnēji programma uzdod jautājumu par lietotāja studiju kursu, kursa numuru, grupu, lietotāja pārlūka valodu, un noskaidro, vai lietotājs izbrauks no vienas vai dažādām adresēm sekojošajā mēnesī. Šo informāciju lietotājs sniedz caur termināli, sekojot iespējamajām norādēm, par to kā ir jāievada informācija.
2. **nodarbības.rtu.lv**
   - Pēc ievadītās informācijas programma izmanto nodarbibas.rtu.lv, lai iegūtu lekciju grafiku, laiku un vietu.
3. **Informācijas ievade Excel Sheet1**
   - Iegūtā informācija par dienām kurās ir lekcijas, cikos tās sākas un beidzas un kur tās notiek, tiek apkopota Excel failā.
4. **GoogleMaps**
   - GoogleMaps tiek ievadīta no Excel attiecīgā informācija un iegūts pārvietošanās maršruts. Katra iterācija ir attiecīgā mēneša diena. Tiek iegūta informācija par to cikos ir attiecīgajās dienās jāiziet no norādītās adreses, uz kurieni (kādu pieturu) jāiet, ar kādu transportu utt.
5. **Informācijas ievade Excel Sheet2**
   - Informāciju ievada Excel failā un saglabājas ar dinamisko nosaukumu.

## Programmas darbības piemērs
Skatiet video par programmas darbību un rezultātu šeit:

### https://youtu.be/8EJe9uKNFsY

## Licence

Šī programmatūra ir licencēta ar MIT licenci. [LICENSE](LICENSE.txt)
