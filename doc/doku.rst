=============
Udako serieak
=============

Serieak karpetaren barnean, fitxategi hauek edukiko ditugu:

- **bootstrap** Bootstrapen osagai guztiak *(ez dugu ikutuko)*
- **doc** Dokumentazioa
- **liburutegia** Hemen edukiko ditugu html-an sartu beharreko osagaiak
- **index.html** Hau seriearen barnean egongo diren artikuluen menua da
- **lehenengoa.html** Hemen kopiatuko dugu lehenengo artikuluaren html-a
- **bigarrena.html** Hemen kopiatuko dugu bigarren artikuluaren html-a
- **hirugarrena.html** Hemen kopiatuko dugu hirugarren artikuluaren html-a
- **laugarrena.html** Hemen kopiatuko dugu laugarren artikuluaren html-a
- **bostgarrena.html** Hemen kopiatuko dugu bostgarren artikuluaren html-a
- **seigarrena.html** Hemen kopiatuko dugu seigarren artikuluaren html-a
- **assets**

  - **css** Igo beharreko css fitxategiak *(ez dugu ikutuko)*
  - **fonts** Webgunerako igoko diren letra tipoak *(ez dugu ikutuko)*
  - **less** Estiloak hemen daude definituak *(ez dugu ikutuko)*
  - **images** Irudiak hemen egongo dira

    - **azala** Azaleko irudiak hemen sartuko ditugu
    - **lehenengoa** Lehenengo artikuluan sartuko diren irudiak
    - **bigarrena** Bigarren artikuluan sartuko diren irudiak
    - **hirugarrena** Hirugarren artikuluan sartuko diren irudiak
    - **laugarrena** Laugarren artikuluan sartuko diren irudiak
    - **bostgarrena** Bostgarren artikuluan sartuko diren irudiak
    - **seigarrena** Seigarren artikuluan sartuko diren irudiak

Edukia sartzeko eman beharreko pausoak
--------------------------------------

Menuan
``````

Titularra sartu
'''''''''''''''

Lehenengo pausoa, headerrean titularra jartzea. *index.html* fitxategian,
*header* etiketak dauden lekuan, *h1* etiketa dagoen lekuan sartu behar da.

    .. code:: html
      <header style="background-image: url('assets/images/azala/azala.jpg');">
        <a class="berria" href="http://berria.eus/udakoak"><img src="assets/images/berria.ico" alt="berria"/> Udako
          Serieak</a>
        <h1 class="line">Titularra titu titu</h1>
      </header>

Azaleko irudia
''''''''''''''

Azaleko irudiak beti *azala.jpg* izena edukiko du eta *assets/images/azala*
karpetaren izenean joango da.

Artikuluen esteketarako txartelak
'''''''''''''''''''''''''''''''''

*card* klasea duen *div*-ak artikulura estekak dituzten txartelak dira. Hasiera
batean bat bakarrik edukiko dugu, eta artikulu gehiago ditugun heinean,
txartel berriak gehituko ditugu, bakoitzean behar diren informazioarekin.

    .. code:: html

      <div class="card">
        <a href="lehenengoa.html" class="cardImage" style="background-image: url('assets/images/lehenengoa/azala.jpg')"></a>
        <h3 class="gaia line"><a href="lehenengoa.html">Lehenengoa</a></h3>
        <p class="gaiaSarrera"><a href="lehenengoa.html">Lorem ipsum dolor sit amet, consectetur
        adipiscing elit. Phasellus et nibh non mi varius eleifend eget quis
        lectus. Nam porttitor sed neque eu pretium.</a></p>
      </div>

Txartelaren argazkia
....................

Txartelaren argazkia, barruan jarriko dugun azalaren argazkiaren berdina izango
da. Hau dela eta, *azala.jpg* deituko dugu eta
*assets/images/artikuluarenzenbakia/* barnean sartuko dugu.

    .. code:: html

        <a href="lehenengoa.html" class="cardImage" style="background-image: url('assets/images/lehenengoa/azala.jpg')"></a>

Txartelaren gaia
................

Artikuluaren gaia edo azpi gaiaren izenburua gehituko dugu hemen eta esteka
aldatuko diogu, tokatzen zaigun artikuluari esteka jarriz.

    .. code:: html

        <h3 class="gaia line"><a href="lehenengoa.html">Lehenengoa</a></h3>

Txartelaren gaiaren sarrera
...........................

Artikuluaren gaiaren sarreratxoa jarriko dugu hemen eta esteka aldatuko diogu,
tokatzen zaigun artikuluari esteka jarriz.

    .. code:: html

        <p class="gaiaSarrera"><a href="lehenengoa.html">Lorem ipsum dolor sit amet, consectetur</a></p>


Artikuluan
``````````

Headerreko irudia
'''''''''''''''''

Azaleko irudiak beti *azala.jpg* izena edukiko du eta
*assets/images/artikuluarenzenbakia* karpetaren izenean joango da.

Artikuluaren kabezera
'''''''''''''''''''''

Liburutegian dagoen *kabezera.html* kopiatuko dugu eta informazio hau gehituko
diogu:

Gaia
....

Gaia sartuko dugu *h3* etiketa eta *gaia* klasea duen izenburuaren barnean.

    .. code:: html

      <h3 class="gaia line">Oposizioaren ikuspegia</h3>

Gaiaren sarrera
...............

Gaiaren sarrera sartuko dugu *gaiaSarrera* klasean duen paragrafoan (*p*).

    .. code:: html

      <p class="gaiaSarrera">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam nec vehicula ante. Donec suscipit facilisis nisi quis euismod. Praesent eu sollicitudin arcu.</p>

Titularra
.........

Titularra *h1* etiketaren barnean sartuko dugu.

    .. code:: html

      <h1 class="titularra">Gris asko, zuri beltzen artean</h1>

Sinadura
........

Sinadura *sinadura* klasea duen paragrafoaren (*p*) barruan sartuko dugu.

    .. code:: html

      <p class="sinadura"><span class="glyphicon glyphicon-pencil"></span> Izena eta Abizena
          <span class="sinadura-data">Arrasate</span></p>

Irudi horizontalak
''''''''''''''''''

Irudi horizontalak bi motatakoak izango dira:

1. **Azpitutalarren azpian doana,** *irudi_horizontala_azpititularra.html*
   fitxategian dagoena kopiatu eta pegatu behar da.

    .. code:: html

      <div class="irudi horizontala">
        <img src="assets/images/lehenengoa/horizontala.jpg"/>
        <label class="oina line">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</label></p>
      </div>

  Irudiaren izena, irudiaren helbidean artikuluaren zenbakia jarri *img src=*, oina eta sinadura bete behar dira.

2. **Testuaren barruan doana,** *irudi_horizontala.html* fitxategian dagoena
   kopiatu eta pegatu behar da nahi den lekuan.

    .. code:: html

      </p>
      <div class="irudi horizontala">
        <img src="assets/images/lehenengoa/horizontala.jpg"/>
        <label class="oina line">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</label></p>
      </div>
      <p class="testua">

  Irudiaren izena, irudiaren helbidean artikuluaren zenbakia jarri *img src=*, oina eta sinadura bete behar dira.

Irudi bertikala
'''''''''''''''

Irudi bertikalak beti testu barruan sartuko dira.
*irudi_bertikala.html* fitxategian dagoena kopiatu eta pegatu behar da nahi
den lekuan.

    .. code:: html

      <span class="irudi bertikala">
        <img src="assets/images/lehenengoa/bertikala.png"/>
        <label class="oina">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</span></label>
      </span>

  Irudiaren izena,, irudiaren helbidean artikuluaren zenbakia jarri *img src=* oina eta sinadura bete behar dira.

Irudi panoramikoa
'''''''''''''''''

Irudi panoramikoak beti testu barruan sartuko dira.
*irudi_panoramikoa.html* fitxategian dagoena kopiatu eta pegatu behar da nahi
den lekuan.

    .. code:: html

      </article>
      <div class="irudi panoramikoa"
           style="background-image: url('assets/images/lehenengoa/panoramikoa.jpg');"/>
        <label class="oina">Hau oina da oina oina oina da hau. <span
            class="sinadura-irudia">Sinadura</span></label>
      </div>
      <article>


  Irudiaren izena, irudiaren helbidean artikuluaren zenbakia jarri *img src=*, oina eta sinadura bete behar dira.

Esanak
''''''

Esanak beti testu barruan sartuko dira. *esanak.html* fitxategian dagoena
kopiatu eta nahi dugun lekuan pegatuko dugu.

    .. code:: html

      </p>
      <section class="esana line">
          <p>Iruñeko espetxe berriaren inauguratu zenean, alderdi guztiek nabarmendu zuten "mugarria" izan zitekeela espetxe arloko eskumenak hartzeko, baina lau urteren ondoren ezer gutxi egin da, Francesen arabera.</p>
          <p class="esanaSinadura">Unai Iturriaga</p>
      </section>
      <p class="testua">

    Esaldia eta izena bete behar dira.

Entresakak
''''''''''

Entresakak beti testu barruan sartuko dira. *entresakak.html* fitxategian dagoena
kopiatu eta nahi dugun lekuan pegatuko dugu.

    .. code:: html

      </p>
      <section class="entresaka line">
        <p>Txosten arabera, erakunde nafarrek aspalditik egin dute aldarrikapen historiko hori. Bere garaian, adibidez, Nafarroako Diputazioak 1923an eskumen hori hartzeko eskatu zion orduko Espainiako Gobernuari.</p>
      </section>
      <p class="testua">
