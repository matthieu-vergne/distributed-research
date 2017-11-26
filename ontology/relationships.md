# Relationships

We provide here the formal relationships we use to formalise our concepts.
If you are not familiar with our formal notation, please look [here](formalisation.md).

## is a

|||
|---|---|
| Description  | The [usual subtyping](https://en.wikipedia.org/wiki/Is-a) relationship, which describes a concept specialisation. |
| Symbol       | ![is_a](http://latex.codecogs.com/gif.latex?is%5C_a) |
| Usage        | ![C1 is_a C2](http://latex.codecogs.com/gif.latex?C1%5C%20is%5C_a%5C%20C2) |
| Consequences | ![C1(x), C1 is_a C2 => C2(x)](http://latex.codecogs.com/gif.latex?C1%28x%29%2C%20C1%5C%20is%5C_a%5C%20C2%20%5Cvdash%20C2%28x%29) |
| Example      | ![Cow(x), Cow is_a Animal => Animal(x)](http://latex.codecogs.com/gif.latex?Cow%28x%29%2C%20Cow%5C%20is%5C_a%5C%20Animal%20%5Cvdash%20Animal%28x%29) |
