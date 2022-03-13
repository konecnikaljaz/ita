# ITA
Naloga 1: Vzpostavitev okolja za nadzor sistema različic

Nakup vinjete

Mikrostoritev sprejema in shranjuje podatke o nakupih vinjet.

![ITA](https://user-images.githubusercontent.com/35294998/158053694-f12d7547-99af-4229-b617-f10d17e8a33e.png)

Funkcionalne | Nefunkcionalne
--- | ---
Sprejemanje, validacija in shranjevanje naročil | Dodajanje novega naročila ne sme trajati več kot 2 sekundi.
Posodobitev starega naročila, v primeru, da uporabnik ustvari novega | Naročila morajo biti arhivirana vsaj 5 let
Vse letne vinjete morajo poteči istočasno, na določen dan v letu | Podatki morajo biti kopirani vsaj na 3 različne lokacije
Vse mesečne in polletne vinjete morajo poteči po pretečenem času nakupa |

Uporabniki

Mikrostoritev dodaja in shranjuje uporabnike, ki so kupili vinjeto.

![ITA (2)](https://user-images.githubusercontent.com/35294998/158054145-15533c00-a6e6-4351-bf1f-d4a3da1307ae.png)



Funkcionalne | Nefunkcionalne
--- | ---
Ob prvem nakupu vinjete se uporabik doda v bazo | Dodajanje novega naročila ne sme trajati več kot 2 sekundi.
Omogočeno mora biti spreminjanje podatkov uporabika, kadarkoli, tudi ko ne kupi nove vinjete | Delovati mora v skladu z GDPR.
Pridobivanje uporabnika glede na številko registerske tablice | Iz sistema mora biti mogoče pridobiti 100 uporabnikov na sekundo, kadar iščemo po registerski tablici.

Zazanavnje veljavnosti

Mikrostoritev pridobo podatke o registerski tablici iz sporočilnega posrednika in ugotovi ali je njegova vinjeta veljavna.

![ITA (1)](https://user-images.githubusercontent.com/35294998/158053993-fbd78dce-8fa8-4fc5-a547-1a638a8b41e6.png)

Funkcionalne | Nefunkcionalne
--- | ---
Sistem se naroči na dogodek zaznavanja nove tablicie večih sporočilnih posrednikov | Sistem se mora odzvati na 100 dogotkov na sekundo.
Sistem mora pridobit podatke iz drugih dveh mikrostoritev in ugotoviti ali je vinjeta zananega vozila veljavna | Do podatkov o zaznanih registerskih tablical lahko dostopajo le pooblaščene osebe.
Sistem mora sporočiti vse registerske tablice, ki niso imele veljavne vinjete, v drugo mikrostoritev | Sistem mora ugotoviti veljavnost vinjete z 100% točnostjo.

