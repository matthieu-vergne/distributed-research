# Concepts

We provide here the list of concepts of our research ontology.
If you are not familiar with our formal notation, please look [here](formalisation.md).

## Peer

|||
|---|---|
| Description   | Individual of the network. |
| Symbol        | ![Peer](http://latex.codecogs.com/gif.latex?Peer) |
| Usage         | ![Peer(x)](http://latex.codecogs.com/gif.latex?Peer%28x%29) |

## User

|||
|---|---|
| Description                   | Local [Peer](#peer). |
| Symbol                        | ![User](http://latex.codecogs.com/gif.latex?User) |
| Usage                         | ![User(x)](http://latex.codecogs.com/gif.latex?User%28x%29) |
| [is a](relationships.md#is-a) | [Peer](#peer) |


## Research Base

|||
|---|---|
| Description   | Database of a [Peer](#peer). It can be local ([User](#user)’s Research Base) or remote (other [Peer](#peer)’s Research Base). |
| Symbol        | ![ResearchBase](http://latex.codecogs.com/gif.latex?ResearchBase) |
| Usage         | ![ResearchBase(x)](http://latex.codecogs.com/gif.latex?ResearchBase%28x%29) |

## System

|||
|---|---|
| Description   | Website, app, or other interface used to access a [Research Base](#research-base) |
| Symbol        | ![System](http://latex.codecogs.com/gif.latex?System) |
| Usage         | ![System(x)](http://latex.codecogs.com/gif.latex?System%28x%29) |

## Research Item

|||
|---|---|
| Description   | Atomic element stored in a [Research Base](#research-base). |
| Symbol        | ![ResearchItem](http://latex.codecogs.com/gif.latex?ResearchItem) |
| Usage         | ![ResearchItem(x)](http://latex.codecogs.com/gif.latex?ResearchItem%28x%29) |

## Motive

|||
|---|---|
| Description                   | Research Item describing the initiator of a research process. |
| Symbol                        | ![Motive](http://latex.codecogs.com/gif.latex?Motive) |
| Usage                         | ![Motive(x)](http://latex.codecogs.com/gif.latex?Motive%28x%29) |
| [is a](relationships.md#is-a) | [Research_Item](#research-item) |

## Question

|||
|---|---|
| Description                   | Motive describing an interrogative expression to be answered, equivalent to the Objective “Have the question X answered.”. |
| Symbol                        | ![Question](http://latex.codecogs.com/gif.latex?Question) |
| Usage                         | ![Question(x)](http://latex.codecogs.com/gif.latex?Question%28x%29) |
| [is a](relationships.md#is-a) | [Motive](#motive) |

## Objective

|||
|---|---|
| Description                   | Motive describing a state of the world to be reached, equivalent to the Question “How to reach objective X?”. |
| Symbol                        | ![Objective](http://latex.codecogs.com/gif.latex?Objective) |0
| Usage                         | ![Objective(x)](http://latex.codecogs.com/gif.latex?Objective%28x%29) |
| [is a](relationships.md#is-a) | [Motive](#motive) |

## Dataset

|||
|---|---|
| Description                   | Research Item describing computable data. |
| Symbol                        | ![Dataset](http://latex.codecogs.com/gif.latex?Dataset) |
| Usage                         | ![Dataset(x)](http://latex.codecogs.com/gif.latex?Dataset%28x%29) |
| [is a](relationships.md#is-a) | [Research_Item](#research-item) |

## Raw Dataset

|||
|---|---|
| Description                   | Dataset describing directly the data. |
| Symbol                        | ![RawDataset](http://latex.codecogs.com/gif.latex?RawDataset) |
| Usage                         | ![RawDataset(x)](http://latex.codecogs.com/gif.latex?RawDataset%28x%29) |
| [is a](relationships.md#is-a) | [Dataset](#dataset) |

## Processed Dataset

|||
|---|---|
| Description                   | Dataset describing a transformation, possibly recursive, of one or more Datasets. |
| Symbol                        | ![ProcessedDataset](http://latex.codecogs.com/gif.latex?ProcessedDataset) |
| Usage                         | ![ProcessedDataset(x)](http://latex.codecogs.com/gif.latex?ProcessedDataset%28x%29) |
| [is a](relationships.md#is-a) | [Dataset](#dataset) |

## Linked Dataset

|||
|---|---|
| Description                   | Dataset describing a link to another Dataset. |
| Symbol                        | ![LinkedDataset](http://latex.codecogs.com/gif.latex?LinkedDataset) |
| Usage                         | ![LinkedDataset(x)](http://latex.codecogs.com/gif.latex?LinkedDataset%28x%29) |
| [is a](relationships.md#is-a) | [Dataset](#dataset) |

## Method

|||
|---|---|
| Description                   | Research Item describing a sequence of steps to execute to satisfy a Motive. |
| Symbol                        | ![Method](http://latex.codecogs.com/gif.latex?Method) |
| Usage                         | ![Method(x)](http://latex.codecogs.com/gif.latex?Method%28x%29) |
| [is a](relationships.md#is-a) | [Research_Item](#research-item) |

## Computable Method

|||
|---|---|
| Description                   | Method which can be automatically executed on a Dataset. |
| Symbol                        | ![ComputableMethod](http://latex.codecogs.com/gif.latex?ComputableMethod) |
| Usage                         | ![ComputableMethod(x)](http://latex.codecogs.com/gif.latex?ComputableMethod%28x%29) |
| [is a](relationships.md#is-a) | [Method](#method) |

## Result

|||
|---|---|
| Description                   | Research Item describing the outcomes of a single execution of a Method. |
| Symbol                        | ![Result](http://latex.codecogs.com/gif.latex?Result) |
| Usage                         | ![Result(x)](http://latex.codecogs.com/gif.latex?Result%28x%29) |
| [is a](relationships.md#is-a) | [Research_Item](#research-item) |

## Computed Result

|||
|---|---|
| Description                   | Result produced by executing a Computable Method. |
| Symbol                        | ![ComputedResult](http://latex.codecogs.com/gif.latex?ComputedResult) |
| Usage                         | ![ComputedResult(x)](http://latex.codecogs.com/gif.latex?ComputedResult%28x%29) |
| [is a](relationships.md#is-a) | [Result](#result) |

## Solution

|||
|---|---|
| Description                   | Research Item closing a research process (i.e. satisfying a Motive) |
| Symbol                        | ![Solution](http://latex.codecogs.com/gif.latex?Solution) |
| Usage                         | ![Solution(x)](http://latex.codecogs.com/gif.latex?Solution%28x%29) |
| [is a](relationships.md#is-a) | [Research_Item](#research-item) |

## Answer

|||
|---|---|
| Description                   | Solution to a Question |
| Symbol                        | ![Answer](http://latex.codecogs.com/gif.latex?Answer) |
| Usage                         | ![Answer(x)](http://latex.codecogs.com/gif.latex?Answer%28x%29) |
| [is a](relationships.md#is-a) | [Solution](#solution) |

## Recipe

|||
|---|---|
| Description                   | Solution to an Objective **(difference with Method?)** |
| Symbol                        | ![Recipe](http://latex.codecogs.com/gif.latex?Recipe) |
| Usage                         | ![Recipe(x)](http://latex.codecogs.com/gif.latex?Recipe%28x%29) |
| [is a](relationships.md#is-a) | [Solution](#solution) |

## Quality Measure

|||
|---|---|
| Description                   | Research Item describing how to evaluate a Research Item in a computable way. |
| Symbol                        | ![QualityMeasure](http://latex.codecogs.com/gif.latex?QualityMeasure) |
| Usage                         | ![QualityMeasure(x)](http://latex.codecogs.com/gif.latex?QualityMeasure%28x%29) |
| [is a](relationships.md#is-a) | [Research_Item](#research-item) |

# About these Concepts

This ontology is designed with the goal of having small, quick to produce [Research Items](#research-item).
The whole point is that the [User](#user) can produce one or few [Research Items](#research-item) even with scarce information or expertise, and submit them to other [Peers](#peer) immediately.
[Quality Measures](#quality-measure) (automatic or manual) can be used to evaluate the quality of a [Research Item](#research-item), thus suggesting improvements to perform.
In other words, we try to avoid the production of whole "papers" or even "drafts", on which the [User](#user) might spend an indefinite amount of time, and push towards immediate sharing of small, fast to write/read content.
