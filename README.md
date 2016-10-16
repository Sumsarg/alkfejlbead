Hetesi Krisztián - CHQQ1O

Tantárgyak felvétele

Funkcionális követelmények:
 -Vendégként a főoldalon szeretnék látni az elérhető tantárgyakat kategóriánként (EA./GY., Matematika/Informatika stb.)
 -Vendégként szeretnék a tantárgyak között szabadon böngészi
 -Vendégként szeretném a tantárgyak időpontjait és termeit látni
 -Vendégként szeretnék konkrét tantárgyra rákeresni
 -Vendégként szeretnék tudni regisztrálni hallgatónak
 
 -Hallgatóként szeretnék tudni bejelentkezni az oldalra
 -Hallgatóként szeretném tudni szerkeszteni a személyes adataimat
 -Hallgatóként szeretnék tudni feljelentkezni a tantárgyak csoportjaiba
 -Hallgatóként szeretném tudni megtekinteni a felvett tantárgyaimat
 -Hallgatóként szeretném tudni leadni vagy módosítani a felvett tantárgyaimat
 
 -Oktatóként szeretnék tudni bejelentkezni az oldalra speciális admin felhasználóval
 -Oktatóként szeretnék tudni új tantárgyat/csoportot felvenni megadott terembe és időpontra
 -Oktatóként szeretnék tudni felvetetni tantárgyat konkrét hallgatóval
 -Oktatóként szeretnék tudni ledobni konkért hallgatót tantárgyakról
 -Oktatóként szeretnék tudni létező tantárgyat megszüntetni
 
Nem funkcionális követelmények:
 -Felhasználóbarát elrendezés, skálázódás bármilyen képernyő méretre
 -Gyors működés
 -Biztonságos működés: jelszavak tárolása, funkciókhoz való hozzáférés
 
 
Szakterületi fogalomjegyzék:
 -Tantárgy: Valamilyen kategóriába eső elfoglaltság, megadott kezdőponttal és teremmel
 -Csoport: Adott tantárgy szét van osztva különböző időpontok és termek szerint csoportokra
 

Szerepkörök:
 -vendég: tantárgyak keresését, böngészését, megtekintését végezheti
 -hallgató: a vendég szerepkörén túl képes felvenni/leadni tantárgyakat és saját beállításait módosítani
 -oktató: a vendég szerepkörén túl képes létrehozni/törölni tantárgyakat és hallgatókat fel illetve lejelentkeztetni róluk
 
 
Oldaltérkép:
 Publikus:
 
 -Főoldal
 -Tantárgyak böngészése
	+Tantárgy megtekintése
 -Belépés
 -Regisztráció
 
 Hallgató:
 
 -Kilépés
 -Profiladatok
	+Profiladatok szerkesztése
 -Felvett tantárgyak megtekintése
 -Tantárgyak böngészése
	+Tantárgy megtekintése
		*Tantárgy felvétele
		
 Oktató:
 
 -Új tantárgy felvétele
 -Tantárgyak böngészése
	+Tantárgy megtekintése
		*Tanuló felvétele
		*Tanuló leadása
		*Tantárgy törlése

		
Végpontok:
 GET /: főoldal
 GET /login: bejelentkező oldal
 POST /login: bejelentkezési adatok felküldése
 GET /profile: profiladatok
 GET /felvett: felvett tantárgyak
 GET /tantargyak: tantárgylista
 GET /tantargyak/:id: tantárgy megtekintése
 GET /tantargyak/create: új tantárgy felvitele, űrlap megjelenítése
 POST /tantargyak/create: új tantárgy felvitele, adatok küldése