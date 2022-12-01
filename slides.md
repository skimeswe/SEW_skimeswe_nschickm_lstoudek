# SEW HTL-Steyr

--

## Stundentafel

---

## 1.Stundentafel - Allgemein



> Quotes are ~~hard~~ easy
> to write - but you can use `code`

---

## 1.Stundentafel - Netzwertechnik

![image](https://user-images.githubusercontent.com/95867717/203752411-982a566d-955e-4c91-a9b7-9a9bc7a2353c.png)

You can freely mix **bold**, *italics*, `code` and normal styles

* normal
* **bold**
* *italics*
* `code`

--

## Lists

---

## Unordered Lists

* a
* b
  * 1
  * 2
    * I
* c

---

## Ordered Lists

automatic numbering

1. a
1. b
    1. 1
    1. 2
1. c

---

## Ordered Lists

custom numbering

1. a  
2. b  
    2.1. 1  
    2.2. 2  
3. c

---

## Definition Lists

(actually: line breaks in long lines in lists...)

* First Term  
This is the definition of the first term.
* Second Term  
This is one definition of the second term.  
This is another definition of the second term.

---

## Font Awesome

*  Itym One<!-- .element: class="mdfa fa-info-circle"--> (this is a feature test in a very long item)
*  Itym Two<!-- .element: class="mdfa fa-question-circle"-->
*  Itym Three<!-- .element: class="mdfa fa-exclamation-circle"-->
*  Itym 4<!-- .element: class="mdfa fa-exclamation-triangle"-->  
with forced line break!

--

## Sprachen und Projekte

---

## C++
C sowie C++ wird als Einstieg in das Programmieren verwendet. C ist einfach zu Lernen. <br />
Danach ist es leichter andere Programmiersprachen wie C++ zu erlernen. 
```c++ 
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}

```



---

## JAVA & JAVAFX
Java ist die am meisten verwendete Programmiersprache im Unterricht und wird in der 3. bis zur 5. Klasse gelehrt. Es werden auch verscheiderne Frameworks wie Java Spring eingesetzt. JavaFX ist eine Erweiterung zum erstellen von Applicationen welches ebenfalls in der 3. Klasse erlernt wird.
```java
public class Main {
    public static void main(String[] args) {
        System.out.println("Hello world!");
    }
}

```
```java
public class HelloApplication extends Application {
    @Override
    public void start(Stage stage) throws IOException {
        FXMLLoader fxmlLoader = new FXMLLoader(HelloApplication.class.getResource("hello-view.fxml"));
        Scene scene = new Scene(fxmlLoader.load(), 320, 240);
        stage.setTitle("Hello!");
        stage.setScene(scene);
        stage.show();
    }

    public static void main(String[] args) {
        launch();
    }
}
```

## Projekte

- Wetter Karte 1 <!-- .element: class="fragment semi-fade-out" data-fragment-index="1" -->
- Raspberry Pi/ LED Cube <!-- .element: class="fragment semi-fade-out" data-fragment-index="2" -->
- Schiffeversenken <!-- .element: class="fragment semi-fade-out" data-fragment-index="3" -->
- Viergewinnt <!-- .element: class="fragment semi-fade-out" data-fragment-index="4" -->
- Live Chat <!-- .element: class="fragment semi-fade-out" data-fragment-index="5" -->
 

---

## Beispiel OpenWeatherMap

![grafik](https://user-images.githubusercontent.com/95867710/205023958-8122f4f9-732a-48dd-914d-a0525dc643bd.png)


---


## SEW - Lehrstoff  

---

## Strukturierte Programmierung 

* Programme mit Hilfe von Methoden oder Funktionen strukturiere und in einer höheren Programmiersprache umsetzen;
* elementare Datentypen und Kontrollstrukturen erläutern sowie geeignete Datentypen für ihre Programme auswählen;
* einfache API-Dokumentationen auf Methodenebene lesen und verstehen;
* einfache Programmbibliotheken für gängige Aufgaben verwenden.

---

 ## Bereich Algorithmen und Datenstrukturen
* einfache Datenstrukturen einsetzen;
* einfache Datenstrukturen sortieren und darin ein Element suchen.

## Bereich Softwareentwicklungsprozess
* mit gängigen Werkzeugen zur Unterstützung der Softwareentwicklung umgehen;
* im Rahmen der Programmentwicklung Fehler finden und beheben;
* einfache Testfälle definieren und damit Programme systematisch testen.

---

## Bereich Strukturierte Programmierung:
Anweisungen und Kontrollstrukturen, elementare Datentypen und Operatoren, prozedurale Programmierung, Benennungskonventionen, API-Dokumentation, Einsatz von Bibliotheken

## Bereich Algorithmen und Datenstrukturen
Einfache Datenstrukturen, Such- und Sortieralgorithmen

## Bereich Softwareentwicklungsprozess
Entwicklungsumgebungen, Testen und Fehlersuche, Debugging

---

## JavaScript

```js [1-2|3|4]
    let a = 1;
    let b = 2;
    let c = x => 1 + 2 + x;
    c(3);
```
```java [1-6|3-5]
public class TheFirst extends Object
{
  
public static void main(String[] args)
  
{
  
}
}
```
---



## JavaScript

```js [1-2|3|4]
    let a = 1;
    let b = 2;
    let c = x => 1 + 2 + x;
    c(3);
```

---

## Callouts 

<!--https://fsymbols.com/signs/bullet-point/-->
```java
String switchExpressionPreview13(Direction way) {
    return switch (way) {                         ➊
        case N -> "Up";                           ➋
        case S -> { yield "Down"; }               ➌
        case E, W -> "Somewhere left or right";
        // default -> "Foo"                       ➍
    };
}
```

- ➊ `switch` can be used as expression
- ➋ `->` instead of `:` → no `break;` necessary!
- ➌ Lambdas can be used to. For _expressions_ they must `yield` a value [version]#13#
- ➍ `default` can be ommitted if a) no expression or b) `enum` with every value handled

---

## Callouts  (Alternative)

<!--https://fsymbols.com/signs/bullet-point/-->
```java
String switchExpressionPreview13(Direction way) {
    return switch (way) {                         ①
        case N -> "Up";                           ②
        case S -> { yield "Down"; }               ③
        case E, W -> "Somewhere left or right";
        // default -> "Foo"                       ④
    };
}
```
- ① <!-- .element: class="co"-->`switch` can be used as expression 
- ② <!-- .element: class="co"-->`->` instead of `:` → no `break;` necessary!
- ③ <!-- .element: class="co"-->Lambdas can be used to. For _expressions_ they must `yield` a value [version]#13#
- ④ <!-- .element: class="co"-->`default` can be ommitted if a) no expression or b) `enum` with every value handled

---

#### Try-with-resources now support „effectively final“ variables

```java
var inputStream = new FileInputStream(".gitignore");
try (inputStream) { … }
```

#### Private methods in Interfaces<!-- .element: class="fragment" data-fragment-index="2" -->

```java
interface Version {
    byte[] digits();
    default String text() { return text(digits()); }
    private String text(byte[] version) { … }
}
```
<!-- .element: class="fragment" data-fragment-index="2" -->

--

## Math

---

## Single Line


`$$ J(\theta_0,\theta_1) = \sum_{i=0} $$`

---

## Multiple lines

`$$\begin{aligned}
  \dot{x} & = \sigma(y-x) \\
  \dot{y} & = \rho x - y - xz \\
  \dot{z} & = -\beta z + xy
  \end{aligned} $$`

--

## Being subtle

* Point a
* Point b   
<span>(but that is not important)</span><!-- .element: class="decent x-small"-->
* Point c

--

## Images

<span>To say it with
[Dilbert](https://dilbert.com/strip/1995-12-10):</span><!-- .element: class="decent x-small"-->

![](https://assets.amuniversal.com/0e1eaf909fcf012f2fe600163e41dd5b)

--

## Transitions

---

<!-- .slide:  data-transition="slide"-->
### The train goes on ...
* none<!-- .element: class="xx-small"-->  
Switch backgrounds instantly
* fade<!-- .element: class="xx-small"-->  
Cross fade — default for background transitions
* slide<!-- .element: class="xx-small"-->  
Slide between backgrounds — default for slide transitions
* convex<!-- .element: class="xx-small"-->  
Slide at a convex angle
* concave<!-- .element: class="xx-small"-->  
Slide at a concave angle
* zoom<!-- .element: class="xx-small"-->  
Scale the incoming slide up so it grows in from the center of the screen

---

<!-- .slide:  data-transition="slide"-->
### and on …
* none<!-- .element: class="xx-small"-->  
Switch backgrounds instantly
* fade<!-- .element: class="xx-small"-->  
Cross fade — default for background transitions

---

<!-- .slide:  data-transition="convex-in concave-out"-->
### and stops.
* fade<!-- .element: class="xx-small"-->  
Cross fade — default for background transitions
* slide<!-- .element: class="xx-small"-->  
Slide between backgrounds — default for slide transitions

---

<!-- .slide:  data-transition="fade-in fade-out"-->
### (Passengers entering and leaving)
* slide<!-- .element: class="xx-small"-->  
Slide between backgrounds — default for slide transitions
* convex<!-- .element: class="xx-small"-->  
Slide at a convex angle

---

<!-- .slide:  data-transition="fade"-->
### And it starts again.
* convex<!-- .element: class="xx-small"-->  
Slide at a convex angle
* concave<!-- .element: class="xx-small"-->  
Slide at a concave angle


