# Scheme-Programming
## Problem 1 <br />
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

## Problem 2 <br />
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

## Problem 3 <br />
![](Problems/problem3.PNG)<br />
* Answer: <br />

#translate numbers to words <br />
(define translate1 (W) <br />
  (cond ((= n 0) ('EMPTY)) <br />
      (else ((> n 19) ( + ( + Y[n // 10] X[n % 10]) W))) <br />
      (else ((>= 19 n) (+ X[n] W))))) <br />

# Helpful slides to undertand more about this scheme programming:
<object data="https://alandix.com/academic/teaching/AI355/pdfs/scheme%20(CSc355%20version)-6up.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="https://alandix.com/academic/teaching/AI355/pdfs/scheme%20(CSc355%20version)-6up.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://alandix.com/academic/teaching/AI355/pdfs/scheme%20(CSc355%20version)-6up.pdf">Download PDF</a>.</p>
    </embed>
</object>
