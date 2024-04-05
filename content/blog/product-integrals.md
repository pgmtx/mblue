+++
title = 'Simplifying product integrals'
date = 2024-04-05T19:04:51+02:00
draft = false
+++

## Introduction

Product integrals are annoying: you have to be extremely careful with varying signs, and recursion makes it even harder.

When I talk about product integration, I mean using this formula:

$$\int{udv}=uv-\int{vdu}$$

## Prostaphaeresis

To find their way, navigators have to calculate angles using a sextant. 

The thing is, the angles can be very, very small (we are expressing them in arcminutes and arcseconds). Let's say that for some reason, you have neither a calculator nor a logarithm table, but per chance, you have a trigonometric book.

This is where prostaphaeresis comes in. It consists of approximating a product by replacing the values by a trigonometric function.

Let \(A\) and \(B\) two very little angles, and \(\cos(a)\) and \(\cos(b)\) their approximation.

You can then use this formula:

$$\cos(a)\cos(b) = \frac{1}{2}(\cos(a+b) + \cos(a-b))$$

There is another one for sine:

$$\sin(a)\sin(b) = \frac{1}{2}(\cos(a-b)-\cos(a+b))$$

Note that these formulas don't have a particular name. Sometimes you can see them referred as Simpson's formulas.
You can also deduce \(\sin(a)\cos(b)\) as well as \(\cos(a)\sin(b)\).

## Trigonometrical formulas

There might be too many, they remain so useful.

$$\sin(x)\cos(x) = \frac{1}{2}\sin(2x)$$
$$\cos^2(x) = \frac{1 + \cos(2x)}{2}$$
$$\sin^2(x) = \frac{1 - \cos(2x)}{2}$$

Keep in mind that whenever you find a powered sine or cosine, you can linearize it to simplify calculations.

## Tabular integration

This technique works with power functions \(x^n\), multiplied by an exponential, a sine or a cosine.

Let's say you have to calculate the following primitive:

$$r=\int x^3\exp(\frac{x}{5})dx$$

You define the function to derivate \(D\) and the one to integrate \(I\).

The goal with \(D\) is to derivate it until you get 0. So \(D\) will be \(x^3\) and \(I\) will be \(\exp(x/5)\).

You have then:

| $$D$$ | $$I$$ |
| :-: | :-: |
| $$x^3$$ | $$\exp(\frac{x}{5})$$ |
| $$3x^2$$ | $$5\exp(\frac{x}{5})$$ |
| $$6x$$ | $$25\exp(\frac{x}{5})$$ |
| $$6$$ | $$125\exp(\frac{x}{5})$$ |
| $$0$$ | $$625\exp(\frac{x}{5})$$ |

Then you multiply and add diagonally, like this.

![](/images/product-integrals/tabular.png)

Don't forget to alternate signs!

So you finally get :
$$r=5x^3\exp(\frac{x}{5})-75x^2\exp(\frac{x}{5})+750x\exp(\frac{x}{5})-3750\exp(\frac{x}{5})$$

You can then factorize by the exponential:
$$r=\exp(\frac{x}{5})(5x^3-75x^2+750x-3750)$$

[Back to top](#introduction)
