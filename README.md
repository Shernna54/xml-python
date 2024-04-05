# xml-python
UF2A1 - Documentació amb Markdown - control

# ***M04 Llenguatge de marques***
## **UF2A1 - Documentació amb Markdown - control**

### *Temas Visualizats a M04 LLengüatge de Marques*
- XML
- DOM
- Python
---
#### XML
![Logo XML](https://www.manualweb.net/img/logos/xml.png)

[XML *(Extensible Markup Language)*](https://www.w3schools.com/xml/) és un llenguatge de marcat dissenyat per emmagatzemar i transportar dades de manera llegible tant per humans com per màquines. S'utilitza per estructurar, emmagatzemar i compartir informació en una varietat d'aplicacions i entorns.
##### Caracteristiques
- **Auto-descriptiu:** Els documents XML contenen dades estructurades en forma d'etiquetes que descriuen el significat de les dades. Això permet que les dades siguin comprensibles fàcilment, tant per humans com per aplicacions informàtiques.

- **Extensible:** XML permet definir conjunts d'etiquetes personalitzades per adaptar-se a les necessitats específiques de qualsevol domini o aplicació. Això fa que sigui molt flexible i adaptable a una àmplia gamma de casos d'ús.

- **Independent del maquinari i del programari:** Els documents XML poden ser creats, processats i compartits en diferents plataformes i amb diferents aplicacions, ja que no estan lligats a cap sistema operatiu o programari específic.

- **Interoperable:** XML proporciona un estàndard comú per representar dades, facilitant l'intercanvi d'informació entre diferents sistemes i aplicacions.

##### XML s'utilitza en una varietat de contextos, incloent:

- **Intercanvi de dades:** XML s'utilitza comúment per intercanviar dades entre sistemes heterogenis, ja sigui a través de la web, mitjançant serveis web o en integracions de sistemes empresarials.

- **Configuració d'aplicacions:** Moltes aplicacions i sistemes utilitzen arxius XML per emmagatzemar configuracions i preferències d'usuari.

- **Representació de documents:** XML s'utilitza per representar documents estructurats, com pàgines web, documents tècnics, llibres electrònics, entre d'altres.

- **Format d'emmagatzematge de dades:** XML es pot utilitzar com a format d'emmagatzematge de dades estructurades, especialment en aplicacions on la llegibilitat humana i la interoperabilitat són importants.

En resum, XML és un llenguatge de marcat versàtil i àmpliament utilitzat que proporciona una forma flexible i estàndard de representar i compartir dades en una varietat d'aplicacions i entorns.

##### Exemple XML
---
```sh
<?xml version="1.0" encoding="UTF-8"?>
<libreria>
  <libro>
    <titulo>El Hobbit</titulo>
    <autor>J.R.R. Tolkien</autor>
    <genero>Fantasía</genero>
    <año>1937</año>
  </libro>
  <libro>
    <titulo>Cien años de soledad</titulo>
    <autor>Gabriel García Márquez</autor>
    <genero>Realismo mágico</genero>
    <año>1967</año>
  </libro>
  <libro>
    <titulo>Orgullo y prejuicio</titulo>
    <autor>Jane Austen</autor>
    <genero>Clásico</genero>
    <año>1813</año>
  </libro>
</libreria>
```



#### DOM

El Document Object Model (DOM) és una interfície de programació d'aplicacions (API) per a documents HTML i XML. Proporciona una representació estructurada del document com un conjunt de nodes i objectes, que els programes poden manipular per a modificar el contingut, l'estil i el comportament del document.

##### Característiques del DOM

- **Estructura jeràrquica**: El DOM organitza els nodes del document en una estructura jeràrquica, amb un node principal que conté tot el document i nodes secundaris que representen els elements, atributs i contingut del document.

- **Accés programàtic**: El DOM proporciona una interfície programàtica que permet als programes accedir, navegar i manipular els nodes del document mitjançant codi JavaScript o altres llenguatges de programació.

- **Actualització en temps real**: Qualsevol canvi realitzat al DOM es reflecteix immediatament en la representació visual del document en un navegador web, el que permet actualitzacions dinàmiques i interactivitat en les pàgines web.

##### Ús del DOM

El DOM s'utilitza principalment en el desenvolupament web per a:

- **Manipulació del contingut**: Canviar el contingut i l'estructura del document HTML o XML dinàmicament mitjançant JavaScript per crear aplicacions web interactives i dinàmiques.

- **Gestió d'esdeveniments**: Capturar i gestionar esdeveniments de l'usuari, com clics de ratolí o presses de teclat, per respondre a la interacció de l'usuari amb la pàgina web.

- **Accés a dades**: Accedir i modificar dades emmagatzemades en formularis web, bases de dades remotes o altres fonts de dades, i actualitzar la pàgina web en conseqüència.

En resum, el DOM és una part fonamental del desenvolupament web modern, que permet la creació d'aplicacions web dinàmiques i interactives mitjançant l'ús de codi JavaScript i altres tecnologies web.

##### Exemple DOM
---
```sh
import xml.dom.minidom

# Carrega el fitxer XML
xml_doc = xml.dom.minidom.parse("datos3.xml")

# Obté una llista amb tots els elements person
persones = xml_doc.getElementsByTagName("person")

# Itera sobre els elements person
for persona in persones:

    id_persona= persona.getAttribute("id")
    tipus_persona= persona.getAttribute("tipus")
    
    # Obté el primer fill (presumiblement el text dins de la etiqueta person)
    nom = persona.getElementsByTagName("name")[0].firstChild.data
    edat = persona.getElementsByTagName("age")[0].firstChild.data
    gènere = persona.getElementsByTagName("sex")[0].firstChild.data
    data_naixement = persona.getElementsByTagName("birth")[0].firstChild.data
    print("|ID:",id_persona,"|Tipus:",tipus_persona,"|Nom:",nom,"|Edat:",edat,"|Gènere:",gènere,"|Data Naixement:",data_naixement)
```

## Python

![Logo Python](https://th.bing.com/th/id/OIP.XNyNyvSu40HljVIJFtOaKQAAAA?w=474&h=474&rs=1&pid=ImgDetMain)

Python és un llenguatge de programació interpretat, de tipus dinàmic i amb una sintaxi elegant i concisa. És utilitzat en una àmplia gamma d'aplicacions, des de desenvolupament web i anàlisi de dades fins a automatització de tasques i programació científica.

##### Característiques de Python

- **Sintaxi clara i llegible**: La sintaxi de Python està dissenyada per ser simple i llegible, el que facilita la creació i comprensió de codi.

- **Tipatge dinàmic**: Python és un llenguatge de tipatge dinàmic, el que significa que no cal declarar explícitament els tipus de dades de les variables.

- **Ampla biblioteca estàndard**: Python inclou una biblioteca estàndard rica i diversa, que proporciona mòduls i funcions per a una àmplia gamma de tasques comunes de programació.

- **Comunitat activa**: Python té una comunitat àmplia i activa de desenvolupadors que contribueixen amb mòduls, llibreries i documentació, el que facilita l'aprenentatge i l'ús del llenguatge.

##### Ús de Python

Python s'utilitza en molts àmbits, incloent:

- **Desenvolupament web**: Frameworks com Django i Flask permeten crear aplicacions web dinàmiques i escalables.

- **Anàlisi de dades**: Biblioteques com NumPy, Pandas i Matplotlib faciliten l'anàlisi i visualització de dades.

- **Automatització de tasques**: Python es pot utilitzar per automatitzar tasques repetitives, com arxivar i processar fitxers, enviar correus electrònics, o interactuar amb bases de dades.

- **Programació científica**: Python és àmpliament utilitzat en la recerca científica i l'enginyeria per a la simulació, el processament d'imatges, la modelització estadística i altres tasques.

En resum, Python és un llenguatge de programació versàtil i popular que s'utilitza en una àmplia gamma d'aplicacions i entorns de desenvolupament.

##### Exemple Python
---
```sh
# Definir dos números
numero1 = 5
numero2 = 3

# Calcular la suma
suma = numero1 + numero2

# Mostrar el resultado
print("La suma de", numero1, "y", numero2, "es:", suma)
```
