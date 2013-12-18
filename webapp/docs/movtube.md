[&#8810;](../README.md) spis treœci

![alt text](resources/img/movtube-logo.png "Logo")
======

1.  <b>Opis modu³u</b></br>
<b>MovtubE</b> to modu³ umo¿liwiaj¹cy publikowanie filmów.
Ka¿dy zarejestrowany u¿ytkownik bêdzie móg³ aktywowaæ ten modu³, a nastêpnie <i><b>umieszczaæ</i></b> filmy dostêpne do <i><b>obejrzenia</i></b> dla ka¿dego. 
U¿ytkownik bêdzie móg³ umieszczaæ filmy <i><b>publiczne</i></b> oraz <i><b>prywatne</i></b>, a co wiêcej przyporz¹dkowywaæ je do œciœle okreœlonych kategorii.<br/>
Pod ka¿dym filmem bêdzie widnia³a iloœæ wyœwietleñ, ocena [Set cookie], data dodania oraz odnoœnik do profilu u¿ytkownika, który umieœci³ film.<br/>
Ka¿dy u¿ytkownik portalu <b>GitBox</b> bêdzie mia³ mo¿liwoœæ <i><b>zg³osiæ</i></b> film, który wg. niego posiada nieodpowiedni¹ treœæ – jest wymagane podanie powodu.<br/>Zg³oszenia u¿ytkowników bêd¹ rozpatrywane pod k¹tem wiarygodnoœci, a nastêpnie odpowiednio karane (b¹dŸ nie).
Ka¿dy film bêdzie filtrowany pod k¹tem umieszczanej treœci (nieodpowiednie filmy bêd¹ usuwane natychmiastowo).

2.  <b>Ograniczenia, formaty, …</b></br>
Maks. czas trwania filmu: 10min
Obs³ugiwane formaty oraz rozdzielczoœæ: [Do ustalenia] 

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
