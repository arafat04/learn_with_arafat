# Time Hierarchy Therorem

Abbreviations: 

Turing Machine $\to$ TM

$\mathb{O}(f(n)) : the function grows at most as fast as $f(n)$
$o(f(n))$ : the function grows strictly slower than $f(n)$

Example:
$f(n)$ : $n \log n$.

So for $\mathbb{O}(f(n))$, the function will grow at most as $f(n) : n \log n$, and for $o(f(n))$, the function will grow strictly slower than $f(n)$. All the functions that grow strictly slower than $\mathbb{O}(f(n))$ are in the set of $o(f(n))$. 

$n \in o\big(n \log n\big), \quad
n \log n \notin o(n)$

It is about in terms computation of algorithms, there is a hierarchy among time complexities.

For any time constructible Function $f : \mathbb{N} \to \mathbb{N}$ there exists a language $\mathbb{A}$ that is decidable by a TM in $\mathbb{O}(f(n))$ time but not in $o(\frac{f(n)}{\log_2 f(n)})$ time. 

### Total Function:

A function $f : \mathbb{N} \to \mathbb{N}$ (it is read $f$ is a function from natural natural to natural number, that is f is a function that takes a natural number as input and returns a natural number as output.) is total  function if for every input x of length $|x|$ = n, a deterministic Turing Machine (TM) halts on x and decide it in $f(n)$ steps. So for every input x, the function is decidable meaning it will halt on every input and either accept or reject it.

$\mathbb{TIME}(f(n))$ is the class of languages which can be decided by a TM in $\mathbb{O}(f(n))$ time.

$\mathbb{TIME}(f(n))$ = {L ∣ L is decidable by a deterministic TM in $\mathbb{O}(f(n))$ time}

**Why this is important for Time hierarchy theorem:**

In order to show there is a hierarchical relation among various time complexities, the TM must able to decide on every input for a language. In this theorem it will only work with the inputs which it can decide, the inputs that are not decidable by the TM, it will be rejected automatically. So the TM does not have to deal with those inputs.

### Time Constructibility:

Time constructible means if we say a function uses $f(n)$ steps to complete the work it is  
