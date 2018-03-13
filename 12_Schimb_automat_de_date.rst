12. Schimb automat de date
===========================

Modulul “ **Schimb automat de date** ” permite schimbul automat al
datelor pastrate in locatii diferite între diverse posturi de lucru
nelimitate ca numar. Fiind incorporat în platforma tehnologică
**1C:Enterprise 8.2**, el permite crearea mai multor baze de date
dispersate geografic, nelimitate ca număr. Exista mai multe scheme
(noduri) de schimb de date cu o baza de date distribuita:ierarhic, cu
multe nivele;topologie stea, etc. Programul oferă mai multe modalităţi
de rezolvare a coliziunilor, în cazul în care informatia este modificata
la diferite noduri ale sistemului distribuit. Schema de schimb de date
este restabilită în cazul refacerii bazei de date din arhivă de rezervă.

**Configurare schimbului de date.** Daca doriti sa setati Calea externa
în alt director sau pe dischetă, faceți click dreapta pe calea externă
și alegeți **Selectie Cale Externă** și căutati directorul în care
doriți să salvați datele. Deschideți **Services** și de la **meniul
Configurație** → **Cale salvare** setați perifericul de salvare pe hard
disk. Catalogul **Configurare schimb de date** este pentru a salva
configurărilor schimburilor de date. Pentru fiecare punct din plan pot
fi create mai multe configurări ale schimbului de date. Conform fiecărei
configurări, schimbul de date poate fi efectuat în regim manual sau în
regim automat. Schimbul de date poate avea două moduri de configurare.
Principiul schimbului de date este la fel pentru toate variantele.
Există o diferenţă doar în modul de transmitere al fişierului pentru
schimbul de date:

-  **Schimb cu ajutorul resursei fisierului.** În momentul configurării
trebuie să indicați catalogul schimbului de date, unde se vor afla
fișierele de schimb intrate și cele ieșite,

-  **Schimb cu ajutorul resursei FTP**. În momentul configurării să
indicați calea catalogului schimbului de date (cu numele serverului).
Poate fi creat un port, login și parolă de acces, pentru fiecare tip
de configurare a schimbului de date susținut funcțional.

Avem următorele posililități:

-  Posibilitatea de a indica cantitatea elementelor din tranzacție la
încărcarea/descărcarea de date (dacă cantitatea e 0, încărcarea și
descărcarea de date se va efectua cu ajutorul unei singure
tranzacții);

-  Posibilitatea de a despacheta mesajele schimbului de date (inclusiv
cele cu parolă);

-  Posibilitatea de a compresa fișierele ieșite ale schimbului de date
(inclusiv cele cu parolă);

-  Posibilitatea de a indica operațiile, care trebuisc executatea la
schimbul de date (încărcare/descărcare de fișiere);

-  Posibilitatea de a introduce un protocol de schimb de date.

Schimbul de date poate fi efectuat automat, lucru pentru care trebui
setată constata Utilizare mecanism schimb de date automat. Dacă constata
respectivă nu este introdusă, schimbul de date automat nu va avea loc.
Un parametru obligatoriu pentru schimbul automat de date este
utilizatorul, pentru care se efectuează schimbul.

Schimbul automat de date poate fi inițializat în 4 cazuri:

-  La lansarea programului. Schimbul de date va avea loc odată cu
lansarea programului;

-  La încheierea sesiunii de lucru cu programul. Schimbul de date va
avea înainte de încheierea sesiunii de lucru cu programul;

-  La validarea catalogului, Schimbul de date se va efectua numai în
cazul în care catalogul, indicat de către utilizator a fost invizibil
până în momentul de față. Configurarea poate fi utilizată pentru
efectuarea schimbului automat de date, în momentul conectării la o
rețea locală sau printr-o cartelă flash. Programul va efectua
periodic o verificare a vizibilității catalogului indicat și va marca
starea acestuia,loc periodic;

-  Schimbul de date periodic. Schimbul de date va avea conform setărilor
suplimentare ale schimbului periodic de date.

Setările schimbului periodic de date:

-  Limitare pe zile ale săptămânii, când trebuie lansat procesul
schimbului periodic de date,

-  Timpul de început al lansării procedurii schimbului periodic. Daca nu
este indicat timpul,schimbul periodic nu va avea loc (va avea loc
numai în cazul în care este precizat faptul că acesta trebuie
lansat),

-  Intervalul de repetare al schimbului automat de date. Se indică
perioada (în minute) la care trebuie repetat procesul de transfer de
dat;

-  Timpul de încetare a schimbului de date. Este determinat momentul în
care trebuie încetată procedura schimbului automat de date.

Mai sunt o serie de setări suplimentare pentru schimbul automat de date:

-  Întrebarea utilizatorului referitoare la începerea schimbului
automat. Aceasta determină dacă e necesar să adresați utilizatorului
o întrebare la începutul sesiunii de schimb de date. Dacă această
opțiune este bifată, schimbul automat va avea loc dacă răspunsul
utilizatorului este pozitiv;

-  Anunțarea erorilor. Aceasta determină dacă informația referitoare la
erorile apărute la efectuarea schimbului de date, trebuie afișată în
fereastra de dialog;

-  Mesaj informațional la efectuarea schimbului automat de date. Aceasta
determină dacă mesajul informațional trebuie afișat în fereastra de
dialog.

Pentru fiecare setare a schimbului automat de date pot fi indicate
câteva condiții suplimentare, conform cărora se poate determina dacă mai
trebuie sau nu efectuat schimbul automat de date. Setările permit
selectarea shimbului de date care trebuie efectuat pentru sesiunea de
lucru din oficiu sau din afara acestuia:

1. Executarea schimbului automat de date doar în cazul în care catalogul
este vizibil;

2. Executarea schimbului automat de date doar în cazul în care catalogul
nu este vizibil;

Schimbul automat de date va avea loc numai în cazul în care catalogul
indicat nu are vizibilitate. Schimbul de date poate fi inițializat
interactiv de către utilizator. Dacă tipul de setare este "**Schimb de
date prin intermediul resursei de fișier**", și nu este creat sau nu
este găsit catalogul schimbului de date, utilizatorului i se va propune
să fie indicat catalogul pentru căutarea fișierului intrat și
descărcării de date.

**Efectuare schimb de date** Cu ajutorul acestei forme poate fi executat
schimbul de date conform unei setări necondiționate a schimbului de
date. Pentru efectuarea schimbului de date, trebuie să selectați setarea
și să apăsați tasta "**Executare".** Există posibilitatea de a adăuga o
setare nouă, pentru care e de ajuns să selectați ultimul punct Adăugare
setare nouă, din lista de setări a schimbului de date. După ce setarea
nouă a fost creată, această va fi selctată automată pentru executare.

În meniul "**Actiuni din formă**", avem punctele:

-  Listă setări schimb de date – permite să treceți la lista de
schimburi de date, deja existente;

-  Aplicarea modificărilor configurației – permite aplicarea asupra
metadatelor a modificărilor configurației, care au apărut în urma
schimbului de date. Se va crea și executa un fișier special bat-file,
conținutul căruia poate fi setat din forma Setare fișier de reînnoire
al configurației. Dacă în timpul procesului de schimb de date la
setarea necondiționată a schibului de date ați primit un mesaj de
eroare: Modificările din configurație sunt obținute în punctul
principal de repartizare IB, după încheierea sesiunii de schimb de
date poate fi utilizată aplicarea autoamată de matadate în
configurație;

-  Setarea de reînnoire al configurației – permite editarea fișierului
bat de reînnoire al configurație.

***Atenție!** Daca pe calculatorul unde veti incarca desenele este
instalata o versiune anterioara de Allplan (ex.: Allplan 2003) atunci
trebuie sa convertiti desenele. Acest lucru se face din **Services
2004,** de la meniul **Fisier Conversie date in versiuni anterioare** +
**selectati** **versiunea (Allplan V16, V17, 2003) alegeti directorul in
care se afla desenele.** Desenele care trebuie convertitite se pot afla
in orice director pe hard disk mai putin in **nemAllplanprj** sau
**nemAllplanSTD.**

