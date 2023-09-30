
user has to select which Algorithm is the best one
depends on
- time
- memory
-> running time should be short and memory should be less used

Running time of an Algorithm depends on how long it takes a complete to run the lines of code of the Algorithm
- speed of computer
- programming language
- compiler & translate

>[!info]
>Asymptotic Notation
>
>>It is a way to describe the behavior of functions in the limit of without bounds

### Asymptotic Grouth

- the rate at which the function grows
- `grouth rate` meaning the complexity of function or the amount of resource it takes up to complete
-> classification of growth

- growing with the same rate: `Theta`
	- C1g(n) <= f(n) <= C2g(n) 
- growing with a slow rate: `Big O`
	- f(n) <= Cg(n) 
- growing with a faster rate: `Omega`
	- Cg(n) <= f(n)

### Theta-notation
- we choose f(n) & g(n) as two differentiate function & say that they have some grouth rate
- f(n) = Theta(g(n))
