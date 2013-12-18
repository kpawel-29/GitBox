[&#8810;](../README.md) spis tre�ci

![alt text](resources/img/movtube-logo.png "Logo")
======

1.  <b>Opis modu�u</b></br>
<b>MovtubE</b> to modu� umo�liwiaj�cy publikowanie film�w.
Ka�dy zarejestrowany u�ytkownik b�dzie m�g� aktywowa� ten modu�, a nast�pnie <i><b>umieszcza�</i></b> filmy dost�pne do <i><b>obejrzenia</i></b> dla ka�dego. 
U�ytkownik b�dzie m�g� umieszcza� filmy <i><b>publiczne</i></b> oraz <i><b>prywatne</i></b>, a co wi�cej przyporz�dkowywa� je do �ci�le okre�lonych kategorii.<br/>
Pod ka�dym filmem b�dzie widnia�a ilo�� wy�wietle�, ocena [Set cookie], data dodania oraz odno�nik do profilu u�ytkownika, kt�ry umie�ci� film.<br/>
Ka�dy u�ytkownik portalu <b>GitBox</b> b�dzie mia� mo�liwo�� <i><b>zg�osi�</i></b> film, kt�ry wg. niego posiada nieodpowiedni� tre�� � jest wymagane podanie powodu.<br/>Zg�oszenia u�ytkownik�w b�d� rozpatrywane pod k�tem wiarygodno�ci, a nast�pnie odpowiednio karane (b�d� nie).
Ka�dy film b�dzie filtrowany pod k�tem umieszczanej tre�ci (nieodpowiednie filmy b�d� usuwane natychmiastowo).

2.  <b>Ograniczenia, formaty, �</b></br>
Maks. czas trwania filmu: 10min
Obs�ugiwane formaty oraz rozdzielczo��: [Do ustalenia] 

3.  <b>Model w bazie danych (BETA)</b></br>
<b>film</b>
* <i>id</i>				(INT/LONG)		[<b>PK</b>]
* <i>id_user</i>		(INT/LONG)		[<b>FK</b>]
* <i>nazwa</i>			(VARCHAR)
* <i>opis</i>			(TEXT)
* <i>plik</i>			(VARCHAR)
* <i>sciezka</i>		(VARCHAR)
* <i>wyswietlenia</i>	(LONG)
* <i>ocena</i>			(DOUBLE .1/.2)
* <i>data_dodania</i>	(DATETIME)

<b>kategoria</b>
* <i>id</i>				(INT/LONG)		[<b>PK</b>]
* <i>nazwa</i>			(VARCHAR)

<b>film_kategoria</b>
* <i>id_film</i>		(INT/LONG)		[<b>FK</b>]
* <i>id_kategoria</i>	(INT/LONG)		[<b>FK</b>]
