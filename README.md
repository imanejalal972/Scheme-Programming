# Scheme-Programming #
## Problem 1 ##
![](Problems/problem1.PNG)<br />
* Answer: <br />

a)  rac in Scheme <br />
(define rac (l) <br />
  (car (reverse l))) <br /> <br />
  
b)  rdc in Scheme <br />
(define rdc (l) <br />
(reverse (cdr (reverse l)))) <br /> <br />

c)  snoc in Scheme <br />
(define snoc (a l) <br />
 (reverse (cons a (reverse l)))) <br /><br /><br />

## Problem 2 ##
![](Problems/problem2.PNG)<br />
* Answer: <br />

a) function simplify in Scheme <br />
(define simplify(l) <br />
  (list(list '+   (lambda (u v)(list '+ (d u) (d v)))) <br />
       (list '-   (lambda (u v)(list '- (d u) (d v)))) <br />
       (list '*   (lambda (u v)(list '+ (list '* u (d v))(list '* (d u) v)))))) <br /><br />
       
b) function remove-noops in Scheme <br />
(define (remove-noops pred l) <br />
 (cond ((null? l) l) <br />
 ((pred (car l)) (remove-noops pred (cdr l))) <br />
 (else (cons (car l) (remove-noops pred (cdr l))))) <br /><br /><br />

## Problem 3 ##
![](Problems/problem3.PNG)<br />
* Answer: <br />

#translate numbers to words <br />
(define translate1 (W) <br />
  (cond ((= n 0) ('EMPTY)) <br />
      (else ((> n 19) ( + ( + Y[n // 10] X[n % 10]) W))) <br />
      (else ((>= 19 n) (+ X[n] W))))) <br />

## Helpful slides to undertand more about this scheme programming: ##
[embed]github.com/pie972/Adversarial-Search/blob/main/Improving%20Monte%20Carlo%20Tree%20Search%20with%20Artificial%20Neural%20Networks%20without%20Heuristics.pdf[/embed]

## WHEN to Contribute? ##
You are ***always welcome*** to contribute.

## HOW to Contribute? ##
- [x] Fork this repository.
- [x] Do your desired changes.
- [x] Make a pull request.
