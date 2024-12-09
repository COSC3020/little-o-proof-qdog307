# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$



#### Formal Definitions:

1. **Little-o definition**:
   $$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$$

2. **Big-O definition**:
   $$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) \le c g(n)$$

---

#### Proof:

1. Assume $f(n) \in o(g(n))$. this means:
   $$\forall c > 0, \exists n_0, \forall n \ge n_0: f(n) < c g(n).$$

2. From this, for any constant $c > 0$, there exists some $n_0$ such that:
   $$\forall n \ge n_0: f(n) < c g(n).$$

3. Since $f(n) < c g(n)$ implies $f(n) \le c g(n)$ we can write:
   $$\exists c > 0, \exists n_0, \forall n \ge n_0: f(n) \le c g(n).$$

4. This satisfies $f(n) \in O(g(n))$.

---

#### Conclusion:

By definition, $f(n) \in o(g(n))$ directly implies $f(n) \in O(g(n))$. Hence:
$$f(n) \in o(g(n)) \implies f(n) \in O(g(n)).$$

#### Sources 

This was not as easy as made out to be, I had to read through a couple of differnet articles and finally watch a youtube video to understand. 
Simialr to Big O but looking at the upper bound. 

https://www.geeksforgeeks.org/analysis-algorithms-big-o-analysis/ 
https://www.geeksforgeeks.org/analysis-of-algorithems-little-o-and-little-omega-notations/ 
https://www.geeksforgeeks.org/types-of-asymptotic-notations-in-complexity-analysis-of-algorithms/ 
https://www.youtube.com/watch?v=Hk_AWLNjGLs 

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.


