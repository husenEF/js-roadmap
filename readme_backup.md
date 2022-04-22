<div align="center">
<h1>Road Map To RN Developer</h1>

<p>ini adalah roadmap untuk belajar menjadi seorang RN developer.
namun ini bukan acuan baku untuk belajar menjadi RN developer.
teman-teman bisa mencari dari refrensi lain.
<strong>semoga membantu</strong>.</p>
</div>

## Daftar Content

<details>
<summary><b>Expand Table of Contents</b></summary>
- Javascrip Dasar
    - [materi 1](#linktomateri 1)
</details>

# Setup

## Prerequisites

Has install all environment

- Source Version Control: Git
- nodejs
- npm/yarn
- Visual Studio Code
- Docker
- ohmyz

## VS Code Extension

1. [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
2. [Git Lens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
3. [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph)
4. [ESlint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

# Repository (GIT)

**Version Control System** (VCS) is a software that helps software developers to work together and maintain a complete history of their work.
**Git** is a distributed version control system for tracking changes in source code during software development.

## Instalation

#### Linux

```bash
$ sudo dnf install git-all

//deb
$ sudo apt install git-all
```

#### Windows

1. download from [git scm](http://git-scm.com)
2. install until finish

## Git Concept

### Repository

A repository is a directory where the project resides. Consider it as a folder in your computer where all the project files are present

### Branch

By default, Git gives us a branch called — `Master` or `Main`. What is a Branch in Git? "**Branch is a lightweight movable pointer to one of the commits**". We can create any number of branches we want and commit our changes to them which remain separated from the other branch.
![branch](https://miro.medium.com/max/1400/1*VFO7otRB-kqg3Y_ImY_IYg.png)

...

## Using GIT

`add how to using git`

# JS Basic

## Variable, Data types

Variable digunakan untuk menyimpan data. Javascript mempunyai 2 type variable mutable & immutable. Mutable bisa menggunakan var dan let, sedangn immutable menggunakan const.

### Var

var bisa menjadi global scoped maupun local, constoh:

```js
var name = 'JS Var'
console.log(name) //expected JS Var
name = 'RN Var`
//expected RN Var
```

masalah `var` adalah dia bisa di akses dari mana saja, karena sifatnya global.

```js
var name = "JS Var";
console.log(name); //expected JS Var
name = "RN Var";
//expected RN Var

if (true) {
  var name = "RN JS Var";
}
console.log(name);
//expected RN JS var
```

solusi bisa mengguna `let`. sedangkan `let` dia ada di dalam block scoped nya.

### Type Data

<details>
<summary>Number</summary>
represented all number type:
<ul>
<li> 10
<li> 11,30
<li> 0133
<li> 0x11
<li> 0b1101
<li> NaN
<li> Infinity/-Infinity
</ul>
</details>

<details>
<summary>Boolean</summary>
Boolean have 2 value, <strong>True</strong> or <strong>False</strong>
</details>
<details>
<summary>String</summary>
<em>update soon</em>
</details>
<details>
<summary>Undefined</summary>
<em>update soon</em>
</details>
<details>
<summary>Null</summary>
<em>update soon</em>
</details>
<details>
<summary>Array</summary>
<em>update soon</em>
</details>
<details>
<summary>Object</summary>
<em>update soon</em>
</details>

## Operator

<table class="">
<tbody><tr>
<th style="width:25%">Operator</th>
<th>Description</th>
</tr>
<tr>
<td>+</td>
<td>Addition</td>
</tr>
<tr>
<td>-</td>
<td>Subtraction</td>
</tr>
<tr>
<td>*</td>
<td>Multiplication</td>
</tr>
<tr>
<td>**</td>
<td>Exponentiation (<a href="https://www.w3schools.com/js/js_2016.asp">ES2016</a>)</td>
</tr>
<tr>
<td>/</td>
<td>Division</td>
</tr>
<tr>
<td>%</td>
<td>Modulus (Division Remainder)</td>
</tr>
<tr>
<td>++</td>
<td>Increment</td>
</tr>
<tr>
<td>--</td>
<td>Decrement</td>
</tr>
</tbody></table>

### JavaScript Comparison Operators

<table >
<tbody><tr>
<th style="width:12%">Operator</th>
<th>Description</th>
</tr>
<tr>
<td>==</td>
<td>equal to</td>
</tr>
<tr>
<td>===</td>
<td>equal value and equal type</td>
</tr>
<tr>
<td>!=</td>
<td>not equal</td>
</tr>
<tr>
<td>!==</td>
<td>not equal value or not equal type</td>
</tr>
<tr>
<td>&gt;</td>
<td>greater than</td>
</tr>
<tr>
<td>&lt;</td>
<td>less than</td>
</tr>
<tr>
<td>&gt;=</td>
<td>greater than or equal to</td>
</tr>
<tr>
<td>&lt;=</td>
<td>less than or equal to</td>
</tr>
<tr>
<td>?</td>
<td>ternary operator</td>
</tr>
</tbody></table>

<em>update soon</em>

## Control Flow

Conditional statements are used to perform different actions based on different conditions.

In JavaScript we have the following conditional statements:

- Use `if` to specify a block of code to be executed, if a specified condition is true
- Use `else` to specify a block of code to be executed, if the same condition is false
- Use `else if` to specify a new condition to test, if the first condition is false
- Use `switch` to specify many alternative blocks of code to be executed

### Conditional (ternary) operator
The conditional (ternary) operator is the only JavaScript operator that takes three operands: a condition followed by a question mark `(?)`, then an expression to execute if the condition is truthy followed by a colon `(:)`, and finally the expression to execute if the condition is **falsy**.
```js
const a = true? 1: 0 //expected 1
``` 
### Switch
alternative for if else
```js
const expr = 'Papayas';
switch (expr) {
  case 'Oranges':
    console.log('Oranges are $0.59 a pound.');
    break;
  case 'Mangoes':
  case 'Papayas':
    console.log('Mangoes and papayas are $2.79 a pound.');
    // expected output: "Mangoes and papayas are $2.79 a pound."
    break;
  default:
    console.log(`Sorry, we are out of ${expr}.`);
}
```
