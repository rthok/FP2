# Final Project Assignment 2: Explore One More! (FP2) 
DUE March 30, 2015 Monday (2015-03-30)

### My Library: 1.4 Plotting Multiple 2D Renderers
Write what you did!
Remember that this report must include:
 
* a narrative of what you did

In this assignement, I worked with the graph plotting library. I made 2-dimensional two graphs. Each graph has two functions with tables that shows what color line corresponds to which function. The first graph plots the functions: 
y = 3x and y= x^2. This graph has the x and y axis going through the graph while the second graph doesn't. The second graph has the functions: cos(x) and sin(x). I've change the style of the line for the cos function so it is dotted instead of a solid line.

* the code that you wrote

```
#lang racket

(require plot)

(define (double x)( * 2 x))
(define (square x)( * x x))
(define (triple x)( * 2 x))
 
;;(plot(function cos(- pi) pi #:label "y = cos(x)" ))

(plot (list(axes)
           (function square -2 2
                     #:label "y = x^2 "
                     #:color "red")
           (function triple -2 2 
                     #:label "y = 3x"
                     #:color "blue")))

(plot (list (function cos (- pi) pi
                      #:label "y = cos(x)"
                      #:color "black"
                      #:style 'dot)
            (function sin (- pi) pi
                      #:label "y = cos(x)"
                      #:color "green")))
   

```
* output from your code demonstrating what it produced

1. [Screen shot of the first graph] (https://github.com/rthok/image/issues/2)
2. [Screen shot of the second graph] (https://github.com/rthok/image/issues/3)

* any diagrams or figures explaining your work 
 
The narrative itself should be no longer than 350 words. Yes, you can add more files and link or refer to them. This is github, handling files is awesome and easy!

Ask questions publicly in the Piazza group.

### How to Do and Submit this assignment

1. To start, [**fork** this repository][forking].
1. Modify the README.md file and [**commit**][ref-commit] changes to complete your solution.
  2. (This assignment is just one README.md file, so you can edit it right in github without cloning)
  3. (You may need to clone and push if you want to add extra files)
1. [Create a **pull request**][pull-request] on the original repository to turn in the assignment.

<!-- Links -->
[piazza]: https://piazza.com/class/i55is8xqqwhmr?cid=411
[schedule]: https://piazza.com/class/i55is8xqqwhmr?cid=453
[markdown]: https://help.github.com/articles/markdown-basics/
[forking]: https://guides.github.com/activities/forking/
[ref-clone]: http://gitref.org/creating/#clone
[ref-commit]: http://gitref.org/basic/#commit
[ref-push]: http://gitref.org/remotes/#push
[pull-request]: https://help.github.com/articles/creating-a-pull-request

