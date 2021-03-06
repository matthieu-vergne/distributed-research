# Relationships

We provide here the formal relationships we use to formalise our concepts.
If you are not familiar with our formal notation, please look [here](formalisation.md).

## has author

|||
|---|---|
| Description   | Relate a [Research Item](concepts.md#research-item) to a [Peer](concepts.md#peer) who created it. |
| Symbol        | ![has_author](http://latex.codecogs.com/gif.latex?has%5C_author) |
| Left operand  | [Research Item](concepts.md#research-item) |
| Right operand | [Peer](concepts.md#peer) |
| Example       | ![Question(q), Peer(John), q has_author John](http://latex.codecogs.com/gif.latex?%5Cbegin%7Balign*%7D%20%26Question%28q%29%5C%5C%20%26Peer%28John%29%5C%5C%20%26q%5C%20has%5C_author%5C%20John%20%5Cend%7Balign*%7D) |

## has parent

|||
|---|---|
| Description   | Relate a [Research Item](concepts.md#research-item) to an immediately previous version. They are not necessarily of the same type, since a [Question](concepts.md#question) can be restated as an [Objective](concepts.md#objective). There might have no parent (creation), 1 parent (modification), or several parents (branch merging). |
| Symbol        | ![has_parent](http://latex.codecogs.com/gif.latex?has%5C_parent) |
| Left operand  | [Research Item](concepts.md#research-item) |
| Right operand | [Research Item](concepts.md#research-item) |
| Example       | ![Question(q1), Question(q2), q2 has_parent q1](http://latex.codecogs.com/gif.latex?%5Cbegin%7Balign*%7D%20%26Question%28q_1%29%5C%5C%20%26Question%28q_2%29%5C%5C%20%26q_2%5C%20has%5C_parent%5C%20q_1%20%5Cend%7Balign*%7D) |

## is a

|||
|---|---|
| Description   | The [usual subtyping](https://en.wikipedia.org/wiki/Is-a) relationship, which describes a concept specialisation. |
| Symbol        | ![is_a](http://latex.codecogs.com/gif.latex?is%5C_a) |
| Left operand  | Concept |
| Right operand | Concept |
| Example       | ![Dataset is_a ResearchItem](http://latex.codecogs.com/gif.latex?Dataset%5C%20is%5C_a%5C%20ResearchItem) |
