<html>

<head>
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
</head>

<body>

<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">attachment
     <font class="fontS"><br>Jeżli chodzi o tworzenie struktury dla attachementow. Powinnien zostać utworzony folder attachment w którym, będzie tworzona struktura stricte wg podanego niżej algorytmu.<br>1) Pobierz 'create_date', 'idattchachment'<br>2) Rozbij 'create_date' na rok, miesiąc, dzień <br>3) Utworz strukture w folderze attachment /rok/miesiac/dzien/idattachment<br>4) Nadaj uprawnienia<br>5) utworz plik <br>6) nadaj uprawnienia<br><br>Pobieranie attachmentu z contentow powinno być zrobione analogicznie:<br>1) Pobierz 'create_date', 'idattachment'<br>2) Utworz stringa attachment/rok/miesiąc/dzień/idattachment<br>3) pobierz z podanego pliku plik.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idattachment</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">content_idcontent</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">status_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(1)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">filename</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(100)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(255)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">create_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">title</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(50)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idattachment<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">attachment_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">content_idcontent<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">banned_ip
     <font class="fontS"><br>Tabela opisująca adresy ip, które zostały z banowane.<br></font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idbanned_ip</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">ip</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(32)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">create_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">expire_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idbanned_ip<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">category
     <font class="fontS"><br>Tabela opisująca posczególne kategorie dostępne dla elementów menu.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idcategory</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">name</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idcategory<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">comment_2
     <font class="fontS"><br>Komentarze dodane przez użytkowników do danego contentu. (B�dzie potrzebne w module bloga)</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idcomment_2</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">status_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(1)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">modification_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">create_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idcomment_2<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">comment_2_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">content
     <font class="fontS"><br>Tabla odpowiadająca za treści dodawane do menu. <br>Należy przyjąć, że w jednym elemencie menu można dodać, tylko jeden content. <br>(Jeżli bedzie taka potrzeba będzie można zmienić na wiele-do-wielu)<br><br></font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idcontent</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">content_type_idcontent_type</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">comment_2_idcomment_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">menu_idmenu</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">status_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(1)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">A - aktywny, kazdy inny string nieaktywny</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">title</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(255)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">header</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(255)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">create_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">hit</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">expire</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">modification_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">rate</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DOUBLE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idcontent<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">content_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">menu_idmenu<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">content_FKIndex2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">content_FKIndex3</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">comment_2_idcomment_2<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">content_FKIndex4</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">content_type_idcontent_type<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">content_type
     <font class="fontS"><br> typ -> Rodzaj contentu<br>1 -> publiczny<br>2 -> prywanty<br>3 -> udost�pniony (tylko dla wybranych użytkowników)<br></font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idcontent_type</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">type_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(1)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idcontent_type<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">logs_2
     <font class="fontS"><br>Tabela przechowująca logi, dotycz�ce nieudanych logowań, oraz rzeczy powiązanych z istotnymi informacjami.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idlogs_2</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">create_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idlogs_2<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">menu
     <font class="fontS"><br>Tabela menu jak wskazuje sama nazwa odpowiada za elementy menu na stronie.<br>Elementy menu na stronie powinny być generowane na podstawie algorytmu:<br>1) Pobierz wszystkie elementy o parent = null<br>2) Po kliknieciu przez użytkownika na dany element menu, pobrać  elementy, które zawierają  parent = klikniety element id<br>3) A następnie sprawdzić, czy dany element menu zawiera contenty (nie jest powiedziane, że element, kt�ry nie będzie niczyjm parentem, ma zawierać jako jedyny content) <br><br>Nie powinno przeładowywać strony, jeżli element menu nie zawiera contentu. </font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idmenu</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">category_idcategory</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">module_idmodule</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">parent</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">Klucz obcy do idmenu</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">title</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(50)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">status_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(1)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">A - aktywny, kazdy inny nieaktywny</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">sort</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">expire</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idmenu<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">menu_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">module_idmodule<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">menu_FKIndex2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">category_idcategory<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">module
     <font class="fontS"><br>Tabela moduł, odpowiada za moduły, które zostały dodane na sztywno.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>idmodule</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">name</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(50)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">idmodule<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">user_account
     <font class="fontS"><br>Tabela opisująca użytkowników na stronie.<br><br>Jedny atrybut wymagający wyjaśnienia, to status:<br>status = 'A' -> User jest aktywny<br>status = 'N' -> Czeka na weryfikacje<br>status = 'B' -> User zbanowany.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>iduser_account</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_description_iduser_description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_type_iduser_type</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">login</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(25)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">password_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(32)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">nickname</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(20)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">status_2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(1)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">A - aktywny, kazdy inny nieaktywny</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">iduser_account<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">user_account_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_type_iduser_type<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">user_account_FKIndex2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_description_iduser_description<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">user_account_has_content_type
     <font class="fontS"><br>Jeżli typ contentu = 3 (Udostąpniony), wtedy tabela będzie przetrzymywać id userów, którzy mają dostęp<br>do contentu</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>user_account_iduser_account</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>content_type_idcontent_type</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account<br>content_type_idcontent_type<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">user_account_has_content_type_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">user_account_has_content_type_FKIndex2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">content_type_idcontent_type<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">user_account_has_module
     <font class="fontS"><br>Wybrane przez usera uruchomione modu�y.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>user_account_iduser_account</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>module_idmodule</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account<br>module_idmodule<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">user_account_has_module_FKIndex1</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">user_account_iduser_account<br></td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">user_account_has_module_FKIndex2</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">Index</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">module_idmodule<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">user_description
     <font class="fontS"><br>description -> Opis dodany przez użytkownika, potrzebny do panelu  ''O mnie"<br>hit -> licznik odwiedzin "O mnie"</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>iduser_description</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">registration_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">ban_date</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">DATE</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">ip</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">VARCHAR(32)</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">hit</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">iduser_description<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
<table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#e4efff">
  <tr>
    <td class="fontX">user_type
     <font class="fontS"><br>Tabela opisująca typy userów<br><br>admin_level -> levele uprawnień: <br>0 -> user<br>1 -> moderator<br>2 -> global moderator<br>3 -> admin<br><br>Role i uprawnienia poszczególnych userów do uzgodnienia.</font></td>
  </tr>
  <tr>
    <td>
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d0dfff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">ColumnName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">DataType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">PrimaryKey&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">NotNull&nbsp;&nbsp;</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">Flags</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Default Value</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="20%">Comment</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="1%">AutoInc</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>iduser_type</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0"><b>INTEGER</b></td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">PK</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">NN</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">AI</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">admin_level</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">INTEGER</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">UNSIGNED </td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">description</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">TEXT</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">&nbsp;</td>
        </tr>

      </table>
    </td>
  </tr>
  <tr>
    <td class="fontB">
      <table cellpadding="2" cellspacing="0" border="0" width="100%" bgcolor="#d8e6ff">
        <tr>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexName</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">IndexType</td>
          <td class="fontSB" style="border-bottom: 1px solid #606060" width="15%">Columns</td>
        </tr>
        <tr>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0" valign="top">PRIMARY</td>
          <td class="fontS" style="border-bottom: 1px solid #C0C0C0">iduser_type<br></td>
        </tr>

      </table>
    </td>
  </tr>

</table>
<br>
<br>
</body>

</html>
