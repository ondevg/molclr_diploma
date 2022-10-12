# molclr_diploma

### The problem
In molecular property prediction tasks, graph neural networks have become a
widely used tool. Recently, self-supervised learning frameworks, especially contrastive
learning, gathered growing attention for the potential to learn molecular representations that generalize to the meaningful chemical space. Unlike supervised, self-supervised learning can directly leverage extensive unlabeled data, which significantly reduces the effort to acquire molecular property labels through costly and time-consuming simulations or experiments. However, most of them do not take
into account the unique cheminformatics (e.g., molecular fingerprints) and multi-level
molecular graph structures (e.g., functional groups).
In toxicity prediction task the molecule substructure can be crucial. Structure
alerts (e.g. toxicophores) are studied pretty well and proved to be responsible for
different types of toxicity. 
### Idea
In this work, we propose chemistry-wise augmentations
for a contrastive learning framework. Two augmentations were implemented: (1)
toxicophore subgraph removal, and (2) toxicophore subgraph saving. This approach
does not violate chemical principles while pushing the model to learn the toxicity-
dependent parts of a molecule.
### Results
Experiments showed that novel augmentations are more efficient than the random subgraph masking approach usually used in molecular contrastive learning. The performance comparison with other GNN-based frameworks is carried out as well.
### Implementation
Based on https://github.com/yuyangw/MolCLR, novel augmentation approach was implemented (for code see dataset folder).
