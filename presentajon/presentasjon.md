# SYSTEK

### Høyne din kodekvalitet med statisk typing og hissig linting

---

### Kodekvalitet - Hvem bryr seg egentlig?

---


* Pleide sitte som herre i egen borg
* global.js &lt; 500 l. kode
* Moderne applikasjon &gt; 10 000 l. kode javascript
* Konsulenttilværelse - oftere bytte
* Ettermæle

---

<img src="http://localhost:1948/_assets/img/nissegrot_pasta.jpg" alt="Pizza" style="width: 400px; height:300px"/>

---


### Årets julegave til deg selv

**Lesbar, forståelig
 og forvaltbar kode**

Note: år du i år tilbake med samme monn:

---

### Hvordan forbedre kodekvalitet?

Note:

Ulike virkemidler

Først se på roten

---

### JavaScript

* Laget med henblikk på validering av forms
* Utviklet til å støtte moderne behov : ES5, ES6, ES2016, ES2017... osv
* jQoery, Lodash, Vue, Ember, Angular, React, Elm

<br />
<img src="http://localhost:1948/_assets/img/pizzabonanza.png" alt="Pizza" style="width: 400px; height:300px"/>



---

### Typiske innvendinger

* Høy grad av fleksibilitet
* Dynamisk språk

> JavaScript, being a dynamic and loosely-typed language, is especially prone to
> developer error. Without the benefit of a compilation process, JavaScript
> code is typically executed in order to find syntax or other errors. Linting tools like ESLint allow developers to discover problems with their JavaScript code without executing it.



---


### Sukre kaka!


Ulike tilnærminger for å oppnå struktur i koden

* dokumentasjon (JSDoc)
* transpilering (Babel)
* compilereing ...

---


* CoffeScript
* LiveScript
* NodeScript (!= Node.JS)
* LispyScript
* ClojureJS/ClojureScript
* Elm
* TypeScript
* Flow

++  mange mange fler


---

### Typer

Enekelte av disse berikelsene tilfører i tillegg til sukker også
statisk typing til JS . Iblant disse er Flow og TypeScript.

---

### Statisk vs dynamisk typing

Statisk typet språk sjekkes ved compile-time 

* Forbedret autofullfør i IDE 
* Større grad av selvdokumentasjon
* Forenkler søk i koden - IDE-en  leder  dirrekte til feks
  funksjonsdefinisjonen
* Reduserer uforutsette feil 

---

### FLOW

Statisk typesjekker for JavaScript

* Du skriver JavaScript
* Legg til FLOW-spesifik annotasjon om typer
* Få løpende feedback

---


#### Eksempel

```javascript
    // @flow
    function square(n: number): number {
       return n * n;
   }

   square("2"); // Error!
```


---


```bash
$ npm install -g flow
$ flow init // > .flowconfig
$ flow status
```

---


---

### Typede vs statisk - fordel ved typere

## FLOW
LOL
## TypeScript
LOL

This is where TypeScript and Flow differ: TypeScript implements both a type
checker and a transpiler that emits plain JavaScript. Flow only does type
checking and relies on Babel or flow-remove-types or some other tool to remove type annotations.

---


Angular > TypeScript (java bakgrunn)
React > Flow

men kan velge selv




---

## Lint - hva er det?

---

[![LINT FLAGG](http://localhost:1948/_assets/img/600px-Flag_of_Lint.svg.png)](http://localhost:1948/_assets/600px-Flag_of_Lint.svg.png)


---

Lint er en kommune i den belgiske provinsen Antwerpen. (WIKI)

---

_Oxford Dictionary_

>Short, fine fibres which separate from the surface of cloth or yarn during processing.
>‘some fabrics leave tiny specks of lint on the glass’


---

### På godt norsk: Lo!

---

I vår verden:

_Statisk analyse av kildekode for å detektere brudd på definerte regler_


---

### Linting i JavaScript

* JSLint - 2002 - Douglas Crockford.  
* JSHint - 2010 - Egentlig en fork av JSLint for  bedre tilpassing av reglene 
* ESLint - 2013 - (industristandard) Laget for at utivklere skal kunne lage engne regler til koden


Note: >>> NOTES Først og fremst online verktøy ibrowser. nå også som cli

---

### Hvorfor linte?

* Fanger opp bugs tidlig
* Hindrer skjulte feil (overskriving av navn, glemt semicolon)
* IDE/Editor-integrasjon > Rask feedback
* Gir mer konsistent kodebase. Ved å ha det som en del av bygget tvinges utviklere til å overholde samme regelverk
* Best practices - hint for roockies
* Fjerner bloat (ubenyttet kode mv)
* Enkelt å sette opp og integrere i eksisterende kodebase
* Enkelt å stramme grepet etter hvert



---

Sinna-linter'n

*
*
*

---

### Hvordan fun
Fra WiKi:  lint is a Unix utility that flags some suspicious and non-portable constructs
Du får
* forhindrer skjulte feil - det ser riktig ut, men feiler i prod
*
* raskere "parsing" / oversikt for utvikler


---

### Hvordan virker det?

https://hackernoon.com/how-linting-and-eslint-improve-code-quality-fa83d2469efe

### JSLint vs JSHint

Hint er en fork av JSLint


---

# END

---

--------------------------------

## EcmaScript vs JavaScript


* “ECMAScript is a standard.”
* “JavaScript is a standard.”
* “ECMAScript is a specification.”
* “JavaScript is an implementation of the ECMAScript standard.”
* “ECMAScript is standardized JavaScript.”
* “ECMAScript is a language.”
* “JavaScript is a dialect of ECMAScript.”
* “ECMAScript is JavaScript.”

( https://medium.freecodecamp.org/whats-the-difference-between-javascript-and-ecmascript-cba48c73a2b5)

---

## EcmaScript
ECMA-262 navnet på er en standard som spesifiserer ECMAScript.
Publisert av Ecma International, første vesjon 1997,  for tiden oppnåd v8 (Juni 2017)


## JavaScript

JavaScript er en dialekt av ECMAScript som forsøker å implementer
spesifikasjonen etter beste evne, men som i noen tilfeller enten ikke makter,
eller velger å gjøre endringer.

JavaScript tolkes igjen av en motor, som er en "vendor spesific" implementasjon av språket.
Dette gjør igjen at hver nettleser implementerer sin måte å tolke JavaScript litt forskjellig
og hver versjon av nettleser har forskjellige ulikheter til standarden(e) de forsøker å støtte.
I tillegg kommer forbrukerenes even (eller mangel på sådan) til å oppdatere sine klienter



For mange er slike språk med på å effektivisere arbeidshverdagen i det man kan
uttrykke seg mer konsist, eller forståelig eller bygge strukturen i koden etter
eget hjerte, MEN en kan ikke utrykke noe mer enn i JavaScript ettersom alt
kompileres ned til JavaScript som igjen tolkes av nettleseren

|



