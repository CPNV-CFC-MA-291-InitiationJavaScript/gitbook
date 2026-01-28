# Java et Javascript

JavaScript et Java se ressemblent sur certains aspects, mais ils sont <mark style="color:orange;">fondamentalement différents l'un de l'autre</mark>. Le langage JavaScript ressemble à Java, mais n'est pas typé statiquement et le <mark style="color:orange;">typage</mark> de JavaScript est faible (alors qu'il est fort en Java). La syntaxe des expressions JavaScript est très proche de celle du Java avec les <mark style="color:orange;">conventions de nommage</mark> et les <mark style="color:orange;">constructions conditionnelles</mark> par exemple : c'est une des raisons qui a fait que le langage LiveScript a été renommé en JavaScript.

```java
//java

import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter first number: ");
        double num1 = sc.nextDouble();
        System.out.print("Enter second number: ");
        double num2 = sc.nextDouble();
        System.out.print("Choose operation (+, -, *, /): ");
        char op = sc.next().charAt(0);

        double result = switch (op) {
            case '+' -> num1 + num2;
            case '-' -> num1 - num2;
            case '*' -> num1 * num2;
            case '/' -> num1 / num2;
            default -> 0;
        };
        System.out.println("Result: " + result);
    }
}


```

```javascript
function calculator() {
    let num1 = parseFloat(prompt("Enter first number:"));
    let num2 = parseFloat(prompt("Enter second number:"));
    let op = prompt("Choose operation (+, -, *, /):");

    let result;
    switch(op) {
        case '+': result = num1 + num2; break;
        case '-': result = num1 - num2; break;
        case '*': result = num1 * num2; break;
        case '/': result = num1 / num2; break;
        default: result = 0;
    }
    alert("Result: " + result);
}
calculator();
```

{% hint style="info" %}
[Faire le laboratoire "Java vs JavaScript"](java-et-javascript.md#java-et-javascript)
{% endhint %}
