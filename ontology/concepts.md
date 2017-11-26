# Concepts

We provide here the list of concepts of our research ontology.

## Peer

|||
|---|---|
| Description   | Individual of the network. |
| Formalisation | Peer(x) |
| Example       | TODO |

## User

|||
|---|---|
| Description   | Local [Peer](#peer). |
| Formalisation | User(x) [is_a](relationships.md#is-a) [Peer](#peer)(x) |
| Example       | TODO |


## Research Base

|||
|---|---|
| Description   | Database of a [Peer](#peer). It can be local ([User](#user)’s Research Base) or remote (other [Peer](#peer)’s Research Base). |
| Formalisation | Research_Base(x) |
| Example       | TODO |
