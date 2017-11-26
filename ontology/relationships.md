# Relationships

We provide here the formal relationships we use to formalise our concepts.

## is a

|||
|---|---|
| Description   | The [usual subtyping](https://en.wikipedia.org/wiki/Is-a) relationship, which describes a concept specialisation. |
| Formalisation | is_a |
| Usage         | C1 is_a C2 |
| Consequences  | C1(x) & C1 is_a C2 => C2(x) |
| Example       | Cow(x) & Cow is_a Animal => Animal(x) |
