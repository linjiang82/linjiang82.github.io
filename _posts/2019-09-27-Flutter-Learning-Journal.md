---
title: Flutter Learning Journal 
categories: Flutter
---
1. All the parameters in Flutter Widget constructor definition are optinal, which means they have to be quoted by curly brace or square brace depending on whether they are named or positional. It is different from Dart which has required and optinal parameters.

2. When see constructor syntax like Constructor(this.a, this.b), it is a syntactic sugar for Constructor(a, b) {this.a=a; this.b=b}
3. MaterialApp widget will create a new Navigator. So when toggle between routes, if the new route also has a MaterialApp, when Navigator.pop, it will go to the closet Navigator and will cause black screen. PLEASE USE SCAFFOLD instead.
4. If Text widget inside a Column, it will only take the minimum space it needs, and when using textAlign to position it to left or right, it would have no effect. One solution is to add 'crossAxisAlignment.start' on Column.
