+++
title = 'Simplifying product integrals'
date = 2024-04-05T19:04:51+02:00
draft = false
+++

## Introduction

Product integrals are annoying : you have to be extremely careful with varying signs, and recursion makes it even harder.

When I talk about product integration, I mean using this formula :

\(a^*=x-b^*\)

## Prostapheresis

To find their way, navigators have to calculate angles using a sextant. 

The thing is, the angles can be very, very small (we are expressing them in arcminutes and arcseconds). Let's say that for some reason, you have neither a calculator nor a logarithm table, but per chance, you have a trigonometrical book.

This is where prostapheresis comes in. It consists of approximating a product by replacing the values by a trigonometrical function.

Let A and B two very little angles, and cos(a) and cos(b) their approximation.

You can then use this formula :

cos(a)cos(b) = (1/2)(cos(a+b) + cos(a-b))

There is another one for sine.

Note that these formulas don't have a particular name. Sometimes you can see them referred as Simpson's formulas.

## Trigonometrical formulas

There might be many, yet they are so useful.

sin(x)cos(x) = (1/2)sin(2x)
cos^2(x) = (1/2)(1 + cos(2x))
sin^2(x) = (1/2)(1 - cos(2x))

## Tabular integration

This technique works with power functions (x^n), multiplied by an exponential, a sine or a cosine.

Let's say you have to calculate the following primitive :

Int(x^3 * exp(x/5))

You define the function to derivate (D) and the one to integrate (I).

The goal with (D) is to derivate it until you get 0. So (D) will be x^3 and (I) will be exp(x/5).

You have then :

| D | I |
| - | - |
| x^3 | exp(x/5) |
| 3x^2 | 5exp(x/5) |
| 6x | 25exp(x/5) |
| 6 | 125exp(x/5) |
| 0 | exp(x) |

Then you multiply and add diagonally, like this.

> Don't forget to alternate signs!

*add image*

So you finally get :

[Back to top](#introduction)
