# Concepts

We provide here the list of concepts of our research ontology.

## Peer

|||
|---|---|
| Description   | Individual of the network. |
| Example       | TODO |
| Formalisation | Peer(x) |

## User

|||
|---|---|
| Description                   | Local [Peer](#peer). |
| Example                       | TODO |
| Formalisation                 | User(x) |
| [is_a](relationships.md#is-a) | [Peer](#peer) |


## Research Base

|||
|---|---|
| Description   | Database of a [Peer](#peer). It can be local ([User](#user)’s Research Base) or remote (other [Peer](#peer)’s Research Base). |
| Example       | TODO |
| Formalisation | Research_Base(x) |

## System

|||
|---|---|
| Description   | Website, app, or other interface used to access a [Research Base](#research-base) |
| Example       | TODO |
| Formalisation | System(x) |

## Research Item

|||
|---|---|
| Description   | Atomic element stored in a [Research Base](#research-base). |
| Example       | TODO |
| Formalisation | Research_Item(x) |

## Motive

|||
|---|---|
| Description                   | Research Item describing the initiator of a research process. |
| Example                       | TODO |
| Formalisation                 | Motive(x) |
| [is_a](relationships.md#is-a) | [Research_Item](#research-item) |

## Question

|||
|---|---|
| Description                   | Motive describing an interrogative expression to be answered, equivalent to the Objective “Have the question X answered.”. |
| Example                       | TODO |
| Formalisation                 | Question(x) |
| [is_a](relationships.md#is-a) | [Motive](#motive) |

## Objective

|||
|---|---|
| Description                   | Motive describing a state of the world to be reached, equivalent to the Question “How to reach objective X?”. |
| Example                       | TODO |
| Formalisation                 | Objective(x) |
| [is_a](relationships.md#is-a) | [Motive](#motive) |

## Dataset

|||
|---|---|
| Description                   | Research Item describing computable data. |
| Example                       | TODO |
| Formalisation                 | Dataset(x) |
| [is_a](relationships.md#is-a) | [Research_Item](#research-item) |

## Raw Dataset

|||
|---|---|
| Description                   | Dataset describing directly the data. |
| Example                       | TODO |
| Formalisation                 | Raw_Dataset(x) |
| [is_a](relationships.md#is-a) | [Dataset](#dataset) |

## Processed Dataset

|||
|---|---|
| Description                   | Dataset describing a transformation, possibly recursive, of one or more Datasets. |
| Example                       | TODO |
| Formalisation                 | Processed_Dataset(x) |
| [is_a](relationships.md#is-a) | [Dataset](#dataset) |

## Linked Dataset

|||
|---|---|
| Description                   | Dataset describing a link to another Dataset. |
| Example                       | TODO |
| Formalisation                 | Linked_Dataset(x) |
| [is_a](relationships.md#is-a) | [Dataset](#dataset) |

## Method

|||
|---|---|
| Description                   | Research Item describing a sequence of steps to execute to satisfy a Motive. |
| Example                       | TODO |
| Formalisation                 | Method(x) |
| [is_a](relationships.md#is-a) | [Research_Item](#research-item) |

## Computable Method

|||
|---|---|
| Description                   | Method which can be automatically executed on a Dataset. |
| Example                       | TODO |
| Formalisation                 | Computable_Method(x) |
| [is_a](relationships.md#is-a) | [Method](#method) |

## Result

|||
|---|---|
| Description                   | Research Item describing the outcomes of a single execution of a Method. |
| Example                       | TODO |
| Formalisation                 | Result(x) |
| [is_a](relationships.md#is-a) | [Research_Item](#research-item) |

## Computed Result

|||
|---|---|
| Description                   | Result produced by executing a Computable Method. |
| Example                       | TODO |
| Formalisation                 | Computed_Result(x) |
| [is_a](relationships.md#is-a) | [Result](#result) |

## Solution

|||
|---|---|
| Description                   | Research Item closing a research process (i.e. satisfying a Motive) |
| Example                       | TODO |
| Formalisation                 | Solution(x) |
| [is_a](relationships.md#is-a) | [Research_Item](#research-item) |

## Answer

|||
|---|---|
| Description                   | Solution to a Question |
| Example                       | TODO |
| Formalisation                 | Answer(x) |
| [is_a](relationships.md#is-a) | [Solution](#solution) |

## Recipe

|||
|---|---|
| Description                   | Solution to an Objective **(difference with Method?)** |
| Example                       | TODO |
| Formalisation                 | Recipe(x) |
| [is_a](relationships.md#is-a) | [Solution](#solution) |

## Quality Measure

|||
|---|---|
| Description                   | Research Item describing how to evaluate a Research Item in a computable way. |
| Example                       | TODO |
| Formalisation                 | Quality_Measure(x) |
| [is_a](relationships.md#is-a) | [Research_Item](#research-item) |

# About these Concepts

This ontology is designed with the goal of having small, quick to produce [Research Items](#research-item).
The whole point is that the [User](#user) can produce one or few [Research Items](#research-item) even with scarce information or expertise, and submit them to other [Peers](#peer) immediately.
[Quality Measures](#quality-measure) (automatic or manual) can be used to evaluate the quality of a [Research Item](#research-item), thus suggesting improvements to perform.
In other words, we try to avoid the production of whole "papers" or even "drafts", on which the [User](#user) might spend an indefinite amount of time, and push towards immediate sharing of small, fast to write/read content.
