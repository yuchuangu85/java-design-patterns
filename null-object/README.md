---
layout: pattern
title: Null Object
folder: null-object
permalink: /patterns/null-object/
categories: Behavioral
tags:
 - Extensibility
---

## Intent
In most object-oriented languages, such as Java or C#, references
may be null. These references need to be checked to ensure they are not null
before invoking any methods, because methods typically cannot be invoked on
null references. Instead of using a null reference to convey absence of an
object (for instance, a non-existent customer), one uses an object which
implements the expected interface, but whose method body is empty. The
advantage of this approach over a working default implementation is that a Null
Object is very predictable and has no side effects: it does nothing.

## Class diagram
![alt text](./etc/null-object.png "Null Object")

## Applicability
Use the Null Object pattern when

* You want to avoid explicit null checks and keep the algorithm elegant and easy to read.

## Credits

* [Pattern Languages of Program Design 3](https://www.amazon.com/gp/product/0201310112/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=0201310112&linkCode=as2&tag=javadesignpat-20&linkId=7372ffb8a4e39a3bb10f199b89aef921)
* [Refactoring to Patterns](https://www.amazon.com/gp/product/0321213351/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=0321213351&linkCode=as2&tag=javadesignpat-20&linkId=2a76fcb387234bc71b1c61150b3cc3a7)
