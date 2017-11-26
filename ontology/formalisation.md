# Ontology Formalisation

This document aims at giving the basics for understanding the formal notations used in this project.
We give a short description of the notation we use, a [second-order logic](https://en.wikipedia.org/wiki/Second-order_logic), and various examples for helping the reader to understand.
If some points are unclear, wrong, or missing, feel free to create an issue or a pull request.

## Concepts

A concept is formally written as a unary relation (function of 1 argument ![f(x)](http://latex.codecogs.com/gif.latex?f%28x%29)) and tell that a particular element corresponds to this concept.
For example, we write that John is a [User](concepts.md#user) through the formula ![User(John)](http://latex.codecogs.com/gif.latex?User%28John%29).
This formula can also be read as "John is an instance of the [User](concepts.md#user) concept".

## Relationships

A relationship is written as an [infix operator](https://en.wikipedia.org/wiki/Infix_notation) and tell that two elements are related to each other in a specific way.
For example, we write that a [Dataset](concepts.md#dataset) [is a](relationships.md#is-a) [Research Item](concepts.md#research-item) through the formula ![Dataset is_a ResearchItem](http://latex.codecogs.com/gif.latex?Dataset%5C%20is%5C_a%5C%20ResearchItem).
The order of the operands is important: ![Dataset is_a ResearchItem](http://latex.codecogs.com/gif.latex?Dataset%5C%20is%5C_a%5C%20ResearchItem) does not mean the same than ![ResearchItem is_a Dataset](http://latex.codecogs.com/gif.latex?ResearchItem%5C%20is%5C_a%5C%20Dataset).
We choosed the infix notation to keep that clear when reading.

## Formula & Inference

Concepts and relationships can be composed into more complex formula to express inferences.
For example, if we know that John is a [User](concepts.md#user), written ![User(John)](http://latex.codecogs.com/gif.latex?User%28John%29),
and that a [User](concepts.md#user) is a [Peer](concepts.md#peer), written ![User is_a Peer](http://latex.codecogs.com/gif.latex?User%5C%20is%5C_a%5C%20Peer),
then we can infer that John is also a [Peer](concepts.md#peer), written ![Peer(John)](http://latex.codecogs.com/gif.latex?Peer%28John%29).
The overall inference can be formally written by listing the premises on the left and deriving (![=>](http://latex.codecogs.com/gif.latex?%5Cvdash)) the consequence on the right:
![User(John), User is_a Peer => Peer(John)](http://latex.codecogs.com/gif.latex?User%28John%29%2C%20User%5C%20is%5C_a%5C%20Peer%20%5Cvdash%20Peer%28John%29)

# Use this Notation in Your Own Contributions

If you want to write with such notation in your issues or pull requests, here are the steps to do:
1. write in your document an image embedder: `![]()`
2. write in the square brackets a textual equivalent of your formula, like `![A -> B]()`
3. go to [this equation editor](http://latex.codecogs.com/eqneditor/editor.php)
4. type the LaTeX formula you want in the editor, like `A \rightarrow B` (use the symbols above the editor for help)
5. wait for the formula to be rendered as an image below the editor
6. copy the URL of the image (right-click on the image + copy URL)
7. insert the URL in the parenthesis, like `![A -> B](http://latex.codecogs.com/gif.latex?A%20%5Crightarrow%20B)`

This example will appear as ![an image](http://latex.codecogs.com/gif.latex?A%20%5Crightarrow%20B) for the browsers able to display images.
The browsers unable to do so will show instead `A -> B`.
