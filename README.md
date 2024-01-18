## Lietojumprogrammatūras automatizēanas rīki projekta README.md
#Projekta uzdevums
Šis projekts ir izveidots ar mērķi automātiski iegūt informāciju par maršrutiem, kas jāveic no lietotāja ievadītās dzīves vietas, līdz RTU ēkām, kur norisināsies lietotāja lekcijas sekojošajā mēnesī. Projektā izmantotas nodarbibas.rtu.lv un Google Maps vietnes. Programma apstrādā lietotāja ievadīto informāciju, automātiski pārlūko nodarbibas.rtu.lv, iegūst lekciju informāciju, un tad izmanto Google Maps, lai aprēķinātu un iegūtu maršrutu no lietotāja norādītās izbraukšanas vietas līdz lekcijas norises vietai. Pēc tam informācija tiek saglabāta Excel failā.

#Izmantotās Python bibliotēkas
selenium: Izmantota, lai automatizētu lietotāja darbību ar tīmekļa pārlūkiem un iegūtu informāciju no nodarbibas.rtu.lv un Google Maps.

openpyxl: Izmantota, lai izveidotu Excel failu, kurā saglabātā informācija par lekciju laikiem, norises vietām un maršrutiem.

unidecode: Nodrošina iespēju stradāt ar latviešu valodā izmantotajiem burtiem.

re: Izmantota adrešu apstrādei.

#Programmatūras izmantošanas metodes
Sākotnēji programma uzdod jautājumu par lietotāja studiju kursu, kursa numuru, grupu, lietotāja pārlūka valodu, un noskaidro, vai lietotājs izbrauks no vienas vai dažādām adresēm sekojošajā mēnesī.

Pēc ievadītās informācijas programma izmanto nodarbibas.rtu.lv, lai iegūtu lekciju grafiku, laiku un vietu.

Iegūtā informācija tiek saglabāta Excel failā, un pēc tam programma izmanto Google Maps, lai aprēķinātu maršrutu no lietotāja norādītās izbraukšanas vietas līdz katras lekcijas norises vietai.

Beigās programma saglabā iegūto informāciju Excel failā, kuram tiek piešķirts nosaukums atkarībā no lietotāja ievadītās studiju programmas nosaukuma.

#Programmas darbības piemērs
Skatiet video par programmas darbību un rezultātu šeit:
https://youtu.be/8EJe9uKNFsY
