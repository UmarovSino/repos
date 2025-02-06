<img src="./images.png">

# javaScript
### lecture2
______

* Condition
* Loops
* Function
_______________
# if-шартгузорӣ
    
3 роҳи сохтани condition мавҷуд аст.
  * бо роҳи if else if else
  * switch case
  * бо роҳи ternary operator

# loop -цыкл
  цылк ҳам ба монанди дар боло зикркардашуда( дар мавзуи if)  бо се роҳ сохта мешавад

* for
* while
* do/while
  

# function-функция

<img src="Снимок экрана 2025-01-08 140406.png">

функция хам ба монанди дигархо ба се гурух чудо карда мешавад:

# fuction declaration

<img src="./Снимок экрана 2025-01-08 140820.png">

функции declaration функцияи номдор мебошад ба воситаи номе ки гузошта мешавад файрот мекнем.

# fuction expression
<img src="./Снимок экрана 2025-01-08 141123.png">

  дар навбати худ ба ду гурух чудо мешавад.

* anonym 
* arrow
  

  намунаи мисолҳо бо ин ду функсия

  <img src="./Снимок экрана 2025-01-08 141624.png">

 # JavaScript Loops
## Loop for
 ### EXAMPLE

```for (let i=0; i<=5; i++) {
    console.log(i);
}
```
 ### While Loop
###EXAMPLE

```let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}
```
### do while Loop
###EXAMPLE

```let i = 0;
do {
    console.log(i);
    i++;
} while (i<=5);```
#JavaScript Functions
# Function Declaration
###EXAMPLE

```function SumTwoNum(num1,num2) {

   return num1+num2;

}
let user1=SumTwoNum(2,3)
console.log(user1);
2. Function Expression
EXAMPLE a. Anonymous Function

let SumTwoNum = function(num1, num2) {
    return num1 + num2;
};
let user1 = SumTwoNum(2, 3);
console.log(user1);
b. Arrow Function

let SumTwoNum = (num1, num2) =>
num1 + num2;
let user1 = SumTwoNum(2, 3);
console.log(user1);
3.IIFE (Immediately Invoked Function Expression)
(function(num1, num2) {
    console.log(num1 + num2);
})(2, 3);
```

<img src="./images.png">

# javaScript
### lecture3
______

<img src="./Снимок экрана 2025-01-10 143408.png">

 ### лексияи сеюм
 _______
<img src="./Снимок экрана 2025-01-10 143423.png">
 
 ### Scope дар ҷава чист?

_______
 Дар JavaScript миқёс бо контексти ҷории рамзи шумо ишора мекунад.Ин контекст муайян мекунад ки дар куҷо мо метавонем ба тағйирёбандаҳо ва функсияҳо дастраси пайдо кунем.
 ________
    Дар навбати худ ба чор гуруҳ ҷудо мешаванд.
  ________
  # Function declaration -Hosting

  <img src="./Снимок экрана 2025-01-10 143535.png">

Дар JavaScript, эъломияҳои функсия комилан баланд карда мешаванд (hoisted). Ин маънои онро дорад, ки ҳам номи функсия ва ҳам таърифи он ба қисми болоии дастрасии худ дар доираи дахлдор бардошта мешаванд, ки функсияро имкон медиҳад дар ҳар куҷои ин доира, ҳатто пеш аз таърифи воқеии он дар код, фаро хонда шавад.
<img src="./Снимок экрана 2025-01-10 143547.png">
Майдони муваққатии беэътиборӣ (Temporal Dead Zone) барои let ва const

TDZ: Ин истилоҳ барои тавсифи ҳолатест, ки дар он тағйирёбандаҳо дастнорас мебошанд. Онҳо дар доира ҳастанд, аммо ҳанӯз эълом нашудаанд. Тағйирёбандаҳои let ва const дар TDZ аз оғози доираи худ то лаҳзаи эълом шуданашон мавҷуданд.

Чӣ тавр TDZ-ро пешгирӣ кардан мумкин аст?
Ба таври нисбатан оддӣ, ҳамеша боварӣ ҳосил кунед, ки let ва const-и худро дар қисми болоии доираи худ таъриф мекунед.

Майдони муваққатии беэътиборӣ:

   * pi; // ReferenceError (Майдони муваққатии беэътиборӣ)
   * const pi = 3.14; (Эълом ва ибтидоисозӣ)
   * pi; // => 3.14 (Дуруст ва коршоям)
  
<img src="./Снимок экрана 2025-01-10 143558.png">





# java Script lecture 4
#### lecture 4
##### recursion 
______

<img src="Снимок экрана 2025-01-14 164955.png">

Рекурсия техникаи худи даъвати функсия мебошад. Ин техника роҳи тақсим кардани мушкилоти мураккабро ба масъалаҳои оддӣ, ки ҳалли онҳо осонтар аст, фароҳам меорад.

Фаҳмидани рекурсия метавонад каме душвор бошад. Беҳтарин роҳи фаҳмидани он, ки чӣ тавр кор мекунад, ин озмоиш бо он аст.
### Ҳолати қатъ
_____
Ҳамон тавре ки ҳалқаҳо метавонанд ба мушкилоти гардиши беохир дучор шаванд, функсияҳои рекурсивӣ метавонанд ба масъалаи рекурсияи беохир дучор шаванд. Рекурсияи беохир он аст, ки функсия ҳеҷ гоҳ занги худро қатъ намекунад. Ҳар як функсияи рекурсивӣ бояд ҳолати боздошта дошта бошад, ки ин шартест, ки функсия худаш занг заданро қатъ мекунад. Дар мисоли қаблӣ, ҳолати қатъкунӣ вақте аст, ки параметр kба 0 табдил меёбад.

Барои беҳтар фаҳмидани консепсия дидани мисолҳои гуногун муфид аст. Дар ин мисол, функсия як қатор рақамҳоро байни оғоз ва анҷом илова мекунад. Шарти боздоштани ин функсияи рекурсивӣ вақте аст, ки анҷом аз start бузургтар набошад ;

 ````Таҳиягар бояд бо рекурсия хеле эҳтиёткор бошад, зеро навиштани функсияе, ки ҳеҷ гоҳ хотима намеёбад ё миқдори зиёди хотира ё қувваи протсессорро истифода мебарад, хеле осон аст. Аммо, вақте ки дуруст навишта шудааст, рекурсия метавонад як равиши хеле муассир ва аз ҷиҳати математикӣ шево ба барномасозӣ бошад.````
 
 <img src="Снимок экрана 2025-01-14 165407.png">

#### мисолҳо арои шарҳ:
~~~~## 1. //MainFunction
function MainFunction(num)
{
   if(num==0) return 1;
   return num*MainFunction(num-1)
}
2.//MainFunction
function MainFunction(num)
{
   if(num==0) return 0;
   return num+MainFunction(num-1)
}
~~~~
# lecture 5
<img src="j1.png">

се намуди string мавҷуд аст.
```
1.double quotes
2.Single  quotes
3.Backticks
```
<img src="j2.png">

Метод дар JavaScript чист?

Усул як блоки кодест, ки танҳо ҳангоми даъват шуданаш кор мекунад. Шумо метавонед маълумотеро, ки бо номи параметрҳо маълум аст, ба усул интиқол диҳед. Усулҳо барои иҷрои амалҳои муайян истифода мешаванд ва онҳоро ҳамчун функсия низ меноманд.
якчанд усулҳо да расм оварда шудаанд.
<img src="j3.png">

методхои чава.
<img src="j4.png">

### charAt[ ]

Усули charAt() аломатро дар индекси (мавқеи) муайяншуда дар сатр бармегардонад. Индекси аломати якум 0, дуюм 1, ... Индекси аломати охирин дарозии сатр - 1 мебошад.

### at[ ]

Усули at() арзиши бутунро мегирад ва Сатри навро бармегардонад. Ин усул имкон медиҳад, ки ададҳои мусбат ва манфӣ дошта бошанд. Ададҳои бутуни манфӣ аз аломати сатри охирин ҳисоб карда мешаванд.

<video src="https://www.youtube.com/watch?v=NXNf9aYTCZ0"></video>


#  lecture 6


<img src="Снимок экрана 2025-01-22 181114.png">

# what is array in javascript?
<img src="Снимок экрана 2025-01-23 170011.png">

#### An array in JavaScript is a type of global object used to store data. Arrays can store multiple values in a single variable, which can condense and organize our code.

#### Массив дар JavaScript як намуди объекти глобалӣ мебошад, ки барои нигоҳ доштани маълумот истифода мешавад. Массивҳо метавонанд арзишҳои сершуморро дар як тағирёбанда нигоҳ доранд, ки метавонанд коди моро конденсатсия ва ташкил кунанд.

<img src="eeee.png">
### методхои массыв да расим боло оварда шудаанд ки хар як ки он вазифахои худро ичро мекунанд

<img src="Снимок экрана 2025-01-23 170500.png">

### механизмхои  js 

  * destructuring assigment
* Spread syntax
* Rest parameters






# Lecture 8

## lecture 8 
* Object 
* Destructuring ,spread
* "`this`" keyword 
* Call,apply,bind

______

<img src="Снимок экрана 2025-01-27 174438.png">



An object is a collection of properties and a property is an association between a name (or key) and a value.


<img src="Снимок экрана 2025-01-27 174634.png">

## Create object{}

Java script object are a nonprimitive data-type that allows you to store multiple collections of data.Object in js are represented as key-value pairs.


## Object methods

* Object.keys()
* object values()
* object.entries()
_____

<img src="Снимок экрана 2025-01-27 175039.png">
