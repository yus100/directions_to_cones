# From Directions to Cones: Multidimensional Representations of Propositional Facts in LLMs

This repository accompanies the paper **"From Directions to Cones: Multidimensional Representations of Propositional Facts in LLMs"**, which introduces and evaluates a method for identifying multi-dimensional activation subspaces (cones) that mediate truth behavior in large language models.

## Overview

Large Language Models can encode factuality internally, even when their outputs are unreliable. Prior work has often approximated truth representations as a single linear direction. We expand on this by discovering **multi-dimensional cones** of activation vectors that collectively influence whether a model responds truthfully to simple propositional prompts.

The key contributions include:

- Demonstrating that truth is mediated not by a single direction but by a subspace of directions.
- Showing that these cones causally affect model responses across multiple architectures and parameter sizes.
- Confirming that cone-based interventions retain unrelated capabilities (e.g., instruction following) with minimal disruption.
- Providing gradient-based optimization methods to discover these cones automatically.

## Key Result Visualization

Below is a visualization of a learned 2D concept cone for truth in residual activation space. Each dot represents a sample direction within the cone and how it modulates output behavior. The three black points mark ablated directions pointing toward specific ground-truth examples.

<p align="center">
  <img src="truth_cone_viz%20(1).png" alt="Concept Cone Visualization" width="400"/>
</p>

## Citation

If you use this work, please cite:

```@inproceedings{
yu2025from,
title={From Directions to Cones: Multidimensional Representations of Propositional Facts in {LLM}s},
author={Stanley Yu and Vaidehi Bulusu and Oscar S. Yasunaga and Clayton Lau and Cole Blondin and Vasu Sharma and Kevin Zhu and Sean O'Brien},
booktitle={ACL 2025 Student Research Workshop},
year={2025},
url={https://openreview.net/forum?id=GYaJKGfmXm}
}
