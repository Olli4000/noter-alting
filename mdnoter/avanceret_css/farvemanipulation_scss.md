# sådan manipulere man med farve i scss ved hjælp af functions

Jeg opretter en variabel med en farve som indhold.
```scss
$awesome-blue: #2196F3;
```
Jeg opretter en regel for a tagget som giver den padding og som giver den en baggrundsfarve, den får farve værdien fra variablen jeg definerede ovenfor.
```scss
a{
	padding: 10px 15px;
	background-color: $awesome-blue;
}
```
jeg opretter en regel for a tagget når jeg holder musen over det, som gør farven den får fra variablen 15% mørkere ved hjælp af darken funktionen.
```scss
a:hover{
	background-color:darken($awesome-blue,15%);
}
```
Den bliver mørkere fordi at den bruger scss funktionen darken, jeg kan gøre den lysere ved at bruge scss funktionen lighten, men der er også mange andre muligheder for farveændring.