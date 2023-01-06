# DOKUMENTÁCIÓ
# Webtech Beadandó

## Szepesi Glória Virág (W0E0RY)

# Kezdőoldal
Kezdő lépésként legeneráltam a feljesztő környezet segítségével egy html szabványt alapként. Ezt bővítettem folyamatosan
A kezdőlapon ("Home" vagy Index.hzml) található egy menüsáv "navbar" néven hivatkozom rá. Itt négy opció közül választhatunk.
Itt a navigációs sáv stílustát a style.css-en belül szabtam meg. Ez a menüsáv biztosítja az átjárhatóságot a négy html oldal között.
Minden felirat alatt a saját oldalának hivatkozása van.
Ez alatt megtalálható egy "szövegdoboz" egy div szerkezetben.

 
## Menüsáv html kódja:
```ruby
<body>
  <header>

    <div class="bg-text">
      <h1 align="center" style="color:rgb(211, 143, 41)">Web Technológiák Beadandó</h1>
      <p h2 align="center" style="color:rgb(194, 62, 62)">Szepesi Glória Virág</p>
    </div>

    <ul class="navbar">
      <li><a href="index.html">Home</a></li>
      <li><a href="lists.html">Lists</a></li>
      <li><a href="form.html">Form</a></li>
      <li><a href="contact.html">Contact</a></li>
    </ul>

  </header>
```
![image](https://user-images.githubusercontent.com/72697467/211065823-1d35b1ef-c01a-49ab-8ea9-06cdd62fc68e.png)


## Menüsáv css style kódja:
```
navbar{
    list-style: none;
    width: 100%;
    height: 30px;
    margin-top: 5px;
    margin-bottom: 0px;
    padding-left: 0px;
    text-align: center;
}

.navbar > li {
    float: left;
    margin-left: 120px;
}

.navbar > li > a {
    color : rgb(211, 143, 41);
    display: block;
    height: max-content;
    font-size: 24px;
    border-radius: 8px;
    text-decoration: none;
    width: 190px;
    
}
```
Középre igazítva létre hoztam egy táblázatot amiben megjelenik az összes htmllel kapcsolatos követelmény. 

## A táblázat:
```ruby
 <table>
    <tr class="center" font="bold">
      <td colspan="5"> <b>Jelen táblázatban megtalálja a teljesítendő feladatokat </b></td>
    </tr>
    <tr>
      <th>Egy soros szöveg beviteli mező
      </th>
      <th>Bepipálható mező</th>
      <th>Rádió gomb</th>
      <th>Színválasztó mező</th>
      <th>Dátumválasztó Mező</th>
    </tr>
    <tr>
      <td>Szöveges beviteli mező</td>
      <td>Checkbox</td>
      <td>Radio button</td>
      <td>Színválasztó</td>
      <td>Dátumválasztó</td>
    </tr>

    <tr class="center">
      <td> <input type="text"></td>
      <td> <input type="checkbox"></td>
      <td><input type="radio"></td>
      <td><input type="color"></td>
      <td><input type="date"></td>
    </tr>
  </table>
  ```
  ![image](https://user-images.githubusercontent.com/72697467/211065754-f8faa2a9-e9e3-4f49-88a3-df37fb397496.png)
  
  Az oldal legutolsó paramétere pedig egy legördülő lista.
  ```ruby
  <d2><strong>Hasznos oldalak programozáshoz</strong></d2>
    <select>
      <option value="StackOvelflow">StackOvelflow</option>
      <option value="GitHub">GitHub</option>
      <option value="W3school">W3school</option>
      <option value="Reddit">Reddit</option>

    </select>
  ```
  
  # Listák
  
  A Menüsor második opciója a "Lists" azaz a listák. Ezen az oldalon megtalálható két lista, egy számozott és egy sima lista. 
  (ordered/ unordered lists)
  
  ## példa a listára:
  ```ruby
    <header>

        <div class="bg-text">
          <h1 align="center" style="color:rgb(211, 143, 41)">Web Technológiák Beadandó</h1>
          <p h2 align="center" style="color:rgb(194, 62, 62)">Szepesi Glória Virág</p>
        </div>
    
        <ul class="navbar">
          <li><a href="index.html">Home</a></li>
          <li><a href="lists.html">Lists</a></li>
          <li><a href="form.html">Form</a></li>
          <li><a href="contact.html">Contact</a></li>
        </ul>
    
    </header>
```

# Form
A Form oldal mint a nevéből is kiderül egy formot jelenít meg. Ide küldhető bármilyen hozzászólás, észrevétel, helyesírási hiba javítás :). 
Ezen az oldaon belül több esetben is internal style-ba szerkesztem az oldalt. A html küdon belül adom meg a stílusjegyeket.
## A From html kódja:

```ruby
    <div class="form">
        <form id="targetForm">
            <span id="formName">Name:</span><br>
            <input id="nameInput" type="text"><br>
            <span id="formDate">Birth date:</span><br>
            <input id="dateInput" type="date"><br>
            <span id="text">Message: </span><br><br>
            <textarea id="textBox" rows="5" cols="30"></textarea><br><br>
            <submit id="sendButton">Send</submit>


        </form>

    </div>
```

## Példa ( Internal Style):
```ruby
.form {
            margin-top: 20%;
            margin-left: 50px;
            border: 10px solid rgb(211, 143, 41);
            width: 300px;
            font-size: 20px;
            padding: 10px;
            color: brown;
        }

        input {
            margin-top: 8px;
            margin-bottom: 5px;
            background-color: rgb(211, 143, 41);
            color: #b628289f;
            font-size: 20px;
        }
```

# Kontakt
Az utolsó html oldal a "Contact" névre hallgat. Ezen az oldalon egy pár sornyi cím található. 

```ruby
    <address>
        Szepesi Glória Virág<br>
        Programtervező informatikus <br>
        Elérhetőség:<br>
        3515, Miskolc, Egyetemváros<br>
        E/4-es kollégium<br>
        első szoba <br>
    </address> 
```

## Erre külön css style található ami kék színűre színezi a szöveget, valamint megnöveli a betűméretet.

```ruby
address{
    margin-top: 20%;
    font-size: larger;
    color: #4682B4 ;
}

```
# CSS- Styling
A css kódban lévő kód határozza meg az egységes részeket a html-ben. Aminek nincs szüksége egyedi stílus igazításra az az eredeti css alapján kerül megformázásra.

## Példa egyedi esetre:
```ruby

.bg-text {
    background-color: rgb(0, 0, 0);
    /* Fallback color */
    background-color: rgba(0, 0, 0, 0.4);
    /* Black w/opacity/see-through */
    color: white;
    font-weight: bold;
    border: 3px solid #f1f1f1;
    position: absolute;
    top: 20%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;
    width: 80%;
    padding: 20px;
    text-align: center;
}
```
## Példa általános esetre:
```ruby
th {
    background-color: #b628289f;
    border: 1px solid rgb(134, 39, 39);
}

tr {
    border: 1px solid black;
}

td {
    border: 1px solid black;
}
```

# JavaScript

A JavaScript segítségével kezelem a formon keresztül bejött inputokat. 
Több funkciója is van a scriptnek. Amennyiben egy mezőt egyáltalán nem vagy helytelen formátummal töltenek ki, azokban az esetekben hibát jelez, üzenetet dob.
Ha minden input helyes abban az eseteben eltárolja az adatokat JSON fájlba lementi.
Amennyiben valamelyik input hibás az elrontott mezőt pirosra színezi át jelezve, hogy melyik nem helyes.

## példa a piros hibajelzésre:
```ruby
function checkCorrectTextBoxValidity(){

    if (textInput.value == "") {
        alert("Message can't be empty");
        text.style.color = "red";
        text.innerText = "Message is empty";

        return false;
    }
    else {
        text.style.color = "#552583";
        text.innerText = "Message: ";
        
        return true;
    }

}
```



























