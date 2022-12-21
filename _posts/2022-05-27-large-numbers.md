---
layout: post
date: 2022-05-27
title: "A Deep Look Into Large Numbers"
mathjax: true
---

When you think of big numbers, what comes to mind? A million? A billion? A googol? or something bigger?
In this post I would like to give you an overview of some big numbers, and some explaination on how we got these big numbers.
**NOTE: My posts will typically not be this long and in depth**

-----
# Simple Numbers
Let's start off with some more basic numbers. A million is $$1,000,000$$ and a billion is $$1,000,000,000$$. A more concise way to write these numbers is using an exponential, like $$10^6$$ and $$10^9$$ which mean $$6$$ zeros and $$9$$ zeros respectively. We can go larger to a googol, which is $$10^{100}$$, or a one with a hundred zeros following it. A "millinillion" is $$10^{3003}$$. However, none of these numbers even come close to a googolplex, or $$10^{googol}$$, a.k.a $$10^{10^{100}}$$, which means a googol zeros. \
\
But, we can go bigger. Currently, we've only been using one or two exponents. Why don't we exponent over and over, or iteravely? Doing this gives us something along the lines of $$10^{10^{10^{10^{10}}}}$$, which we can replace with a googolplex to make $$googolplex^{googolplex^{googolplex^{googolplex^{googolplex}}}}$$. Another operation we can use is a factorial ($$!$$). This just means multiply all the positive whole numbers less than or equal to it together. An example is $$4! = 4 * 3 * 2 * 1 = 24$$. So, we can take our previous number and factorial it: $$googolplex^{googolplex^{googolplex^{googolplex^{googolplex}}}}!$$, or add factorials multiple times: $$googolplex^{googolplex^{googolplex^{googolplex^{googolplex}}}}!!!!!!$$

## Large Constants
There are also some huge constants, such as <a href="https://en.wikipedia.org/wiki/Steinhaus%E2%80%93Moser_notation#Moser's_number">Moser's number</a>, <a href="https://en.wikipedia.org/wiki/Skewes%27s_number">Skewes's number</a> and <a href="https://en.wikipedia.org/wiki/Graham%27s_number">Graham's number</a>. I will cover Graham's number in the next section, however the first two are less important and far smaller than our next numbers.

# Advanced Numbers
Now we're getting quite big, so we're going to have to get more advanced with how we're setting this up. We can't simply write out a googol number of factorials and exponents by hand, as that would take forever. In order to overcome that, we invented some mathematical notations. I will quickly cover them and then jump into the big numbers. The notations that I'll be using here are Knuth's Up Arrow Notation and Conway's Chained Arrow Notation. Knuth's Up Arrow Notation is defined so that $$m\uparrow n = m^n$$ and $$m\uparrow\uparrow n = \underbrace{m \uparrow (m \uparrow m \uparrow (...))}\_n = \underbrace{m^{m^{m^{.^{.}}}}}\_n$$. In addition to this, there is also the format $$m\uparrow^x n$$ which means $$m \underbrace{\uparrow ... \uparrow}\_x n$$. Conway's chained arrow notation is equivalent to the second format, so that $$m \to n \to x = m\uparrow^x n$$. \
\
Now that we have covered these notations, we can start looking at some huge numbers. Graham's number is huge, far far greater than our previous numbers, and it is also interesting in the way it is defined. Graham's number $$G = g_{64}$$ where $$g$$ is defined as $$g\_n = \left\{\begin{matrix} 3 \uparrow \uparrow \uparrow \uparrow 3, & n=1 \\\\ 3 \uparrow^{g_{n-1}} 3, & n \geq 2, n \in \mathbb{N} \\\\ \end{matrix}\right.$$. Now, this definition may look a bit scary, but it is simpler than it looks. When $$n=1$$, $$g\_n=3 \uparrow \uparrow \uparrow \uparrow 3$$, and when it is a positive whole number that is greater than or equal to two, it is defined as $$3 \uparrow^{g_{n-1}} 3$$. So, you can see why Graham's number $$G$$ is huge: we are repeating this arrow notation over and over 64 times. The bounds for $$G$$ are $$3 \to 3 \to 64 \to 2 < G < 3 \to 3 \to 65 \to 2$$. With the definition of $$g$$ you can also go bigger, so for an example let's set our current biggest number to $$g\_{\_G}$$.
\
Another cool thing you can do related to up arrow notation are Ackermann Numbers, which are defined as $$n \uparrow^n n, n \in \mathbb{W}$$, or $$n \uparrow^n n$$ while $$n$$ is a whole number. The Ackermann Numbers start small, but grow big fast. Defining a function $$A(n) = n \uparrow^n n$$, or $$A(2)$$ giving you the second Ackermann number, for example. $$A(1) = 1$$ and $$A(2) = 4$$, but at $$A(3)$$ it jumps to a huge $$\underbrace{3^{3^{.^{.^{.^3}}}}}\_{7,625,597,484,987}$$. So, to continue our huge numbers let's take our number $$g\_{\_G}$$ and plug it into $$A$$ which becomes $$A(g\_{\_G})$$. This number is so huge it's almost impossible to even describe.
\
Well, we applied our function earlier, so what are some other functions we can use? Well, there's the TREE function which is defined as finding the largest $$m$$ for $$TREE(n), n \in \mathbb(N)$$ so that there is a sequence $$T_1...T_m$$ of rooted trees labelled from $$n$$ labels where each $$T_i$$ has a maximum of $$i$$ vertices so that $$T_i \nleq T_j$$ for any $$i < j \leq m$$. Now, this definition is very complicated but for the sake of this article let's just say that this is a function that grows EXTREMELY fast, which makes our current number seem small. So, we can now plug our number in and get $$TREE(A(g\_{\_G}))$$. There is one last function that we will use here, the famous $$RAYO(n)$$ function. This function takes a number $$n$$ and describes the act of getting the biggest number non-infintesimal that fits in $$n$$ symbols in first order set theory. This function is used to get Rayo's number, the current largest non-infintesimal non-transfinite number we know (created in a unique manner), which is $$RAYO(10^{100})$$. Finally, we can take our number and plug it in to create $$RAYO(A(g\_{\_G}))$$, therefore creating the biggest number.

# Conclusion
We have created some extremely huge numbers and covered some big functions, but it is important to realize that you can always add one to your answer. For those who say "infinity", typically mathematicians say that infinity is a concept, not a traditional number, although there are some cool things like $$\aleph_0$$, $$\omega_{\omega_{\omega_{...}}}$$, and $$\epsilon_{\epsilon_0}$$. Big numbers are cool to research and look at and are a great challenge to wrap our heads around. If you liked this post I would highly recommend looking at the things I haven't covered here, namely transfinite numbers, uncomputable numbers, fast-growing heriarchies, and the different levels of infinity. 

## See Also / Further Reading
- [List of all numbers (Official)](http://www.mrob.com/pub/math/largenum.html)
- [Transfinite numbers](https://en.wikipedia.org/wiki/Transfinite_number)
- [Busy Beaver function](https://en.wikipedia.org/wiki/Busy_beaver)
- [Ackermann function (Wikipedia)](https://en.wikipedia.org/wiki/Ackermann_function)
- [Ackermann function (Wolfram MathWorld)](https://mathworld.wolfram.com/AckermannFunction.html)
- [Fast growing heriarchy](https://en.wikipedia.org/wiki/Fast-growing_hierarchy)
- [Levels of infinity (Video)](https://www.youtube.com/watch?v=SrU9YDoXE88)

-----
### References
- [Names of large numbers](https://en.wikipedia.org/wiki/Names_of_large_numbers)
- [Googol](https://en.wikipedia.org/wiki/googol)
- [Googolplex](https://en.wikipedia.org/wiki/googolplex)
- [Factorial](https://en.wikipedia.org/wiki/Factorial)
- [Factorial Plot/List](https://www.wolframalpha.com/input?i=factorial)
- [Moser's Number](https://en.wikipedia.org/wiki/Steinhaus%E2%80%93Moser_notation#Moser's_number)
- [Skewes's Number](https://en.wikipedia.org/wiki/Skewes%27s_number)
- [Graham's Number](https://en.wikipedia.org/wiki/Graham%27s_number)
- [Knuth's Up Arrow Notation (Wikipedia)](https://en.wikipedia.org/wiki/Knuth%27s_up-arrow_notation)
- [Knuth's Up Arrow Notation (Wolfram MathWorld)](https://mathworld.wolfram.com/KnuthUp-ArrowNotation.html)
- [Conway's Chained Arrow Notation (Wikipedia)](https://en.wikipedia.org/wiki/Conway_chained_arrow_notation)
- [Ackermann Number (Wolfram MathWorld)](https://mathworld.wolfram.com/AckermannNumber.html)
- [Ackermann Number (WolframAlpha)](https://www.wolframalpha.com/input?i=Ackermann+Number)
- [TREE function definition and TREE(3)](https://en.wikipedia.org/wiki/Kruskal%27s_tree_theorem#TREE(3))
- [Rayo's Number and RAYO function](https://en.wikipedia.org/wiki/Rayo%27s_number)

### Unofficial big number list
- [List of huge numbers](https://bignumbers.fandom.com/wiki/List_of_numbers)
- [Uncomputable numbers](https://googology.fandom.com/wiki/List_of_googolisms/Uncomputable_numbers)
