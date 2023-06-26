# Compositional Abstractions Tutorial

Welcome!

This tutorial is based on work we presented at the 2021 Cognitive Science Conference. Find the paper [here](https://cogtoolslab.github.io/pdf/mccarthy_cogsci_2021b.pdf). The goal of this project is to model the change in language as people learn to communicate about a shared procedural task-- recreating a scene of block towers.

We recommend reading this intro before diving into the tutorial. Here you will find a more detailed description of the experiment and a high-level description of the model. The tutorial itself is split across three notebooks, which you can find in the `notebooks` folder.

## Experiment

In our experiment, participants were paired up and assigned the role of Architect or Builder. Their shared goal was to accurately recreate target scenes consisting of two block towers.

<p style="font-size: smaller;  text-align: center;">
  <img width="70%" src="img/task.png" style=""></img> </p>

*Architects* were shown the target scenes. They had to sent text instructions to the Builder, explaining how to construct the current scene.  
*Builders* could not see the scenes. They followed the Architect's instructions by placing blocks in a Building environment.

In the [first notebook](/notebooks/ca_language.ipynb), we analyze Architects' language to show that it becomes more abstract over time. Most saliently, we find the emergence of language referring to larger entities in the scenes, in particular to the three block towers that recurred across scenes:

<p style="font-size: smaller;  text-align: center;">
  <img width="30%" src="img/task_towers.png" style=""></img> </p>


## Model

Our computational model consists of two key steps that both rely on *programmatic representations* of construction procedures. Representing procedures as programs enables us to capture the hierarchical structure of the task and the abstractions that emerge in language.

We first model the learning of part concepts as the acquisition of *program fragments*-- functional substrings of a program that represent subprocedures. Learning these abstractions allows scene programs to be rewritten more concisely. In the [second notebook](/notebooks/ca_programs.ipynb), we show how this process can be implemented using a specific program abstraction algorithm.

The second key component of our model is a Bayesian model of convention formation. The crucial idea here is that, although someone may in principle have the representational capacity to communicate in a very concise way, they will only do so if they have a reason to believe that their partner will understand them. In the [third notebook](/notebooks/ca_conventions.ipynb), we explore how people may trade-off between conciseness and informativity of their language, by modeling how people form ad-hoc conventions for referring to learned abstractions.

## Tutorial

This tutorial is split across three notebooks.

- [Notebook 1: Exploring abstraction in language about building](/notebooks/ca_language.ipynb)
- [Notebook 2: Learning part concepts with program abstractions](/notebooks/ca_programs.ipynb)
- [Notebook 3: Forming conventions to talk about shared abstractions](/notebooks/ca_conventions.ipynb)

Each can be tackled separately, however, they are designed to be run in order.

## Installation
