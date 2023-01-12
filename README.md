# AttentionCrossTranslation
## Unsupervised cross-domain translation via deep learning and adversarial attention neural networks and application to music-inspired protein designs

Markus J. Buehler, Massachusetts Institute of Technology, 77 Massachusetts Ave., Cambridge, MA 02139, USA

E-mail: mbuehler@MIT.EDU 

**Summary**: Taking inspiration from nature about how to design materials has been a fruitful approach, used by humans for millennia. A persistent challenge, however, is the translation of information across disparate domains – such as, using mechanisms found in the construction of language or music, to yield paradigms for structural engineering, polymer design, or protein engineering.  Translations of this type have remained elusive given the high degree of complexity that different representations have, combined with a lack of knowledge of how distinct representations relate. The problem is particularly challenging because a priori, there typically exist no known associations between the two representations so that conventional scientific assessments cannot be conducted due to a lack of pairings of elements of the two domains. In this paper we address an elementary problem underlying this class of problems, to discover how patterns seen in disparate domains can be related using a computationally rigorous approach. Using a deep learning approach based on a cycle consistent attention neural network architecture, we report a method that identifies such relationships directly from data, without any knowledge of relationships or labels. The approach is first validated with a set of known translation problems, and then used to discover a mapping between musical data – based on the corpus of note sequences contained in J.S. Bach’s Goldberg Variations created in 1741 – and protein sequence data – information sampled more recently over the past decades. Since the translations are cycle- and self-consistent, the approach offers a bidirectional translation of information, and the technique offers an unsupervised strategy to discover translations across disparate knowledge domains. Using protein folding algorithms, 3D structures of the predicted protein sequences are generated and their stability is validated using explicit solvent molecular dynamics (MD). Conversely, musical scores generated from protein sequences are sonified and rendered into audible sound. 

**The Bigger Picture**:  Human creativity has advanced the way we understand the world; including scientific and artistic modalities. However, until now, the convergent use of disparate knowledge bases has remained elusive, especially connecting art and science. This is partly due to the fact that translating insights across distinct domains is not yet possible. To address this challenge, we report a method to achieve such translations using deep learning, whereby salient relationships are discovered in an unsupervised fashion, without knowledge of pairing or domain knowledge, thereby expanding the concept of bio-inspiration to encompass vast swaths of human knowledge. The method is demonstrated in the reversible, bidirectional translation of musical data (based on Bach’s Goldberg Variations) to protein sequences, discovered in a fully autonomous manner. The general method has broader applications for other discovery platforms in a variety of engineering, scientific, cultural, artistic and environmental data, opening many possibilities for further experimental and computational studies of pattern engineering.   

Published in: Patterns, 2023

![image](https://user-images.githubusercontent.com/101393859/212066094-9de67fd9-f2de-4dfa-b04d-4909f5fb2ee8.png | width=100)

#### Dataset: 
https://www.dropbox.com/s/51v2texurkstwjv/Goldberg_extended_256.npy?dl=0
https://www.dropbox.com/s/xb3jfj43wy1po8k/Protein_extended_256.npy?dl=0 

#### Weights:
https://www.dropbox.com/s/6ipt5mmuc2ebjjs/V0.628_checkpoint_1010.zip?dl=0

## Getting Started

1) Open AttentionCrossTranslation.ipynb
2) Download dataset and/or model weights (links above and in notebook)
3) Execute notebook

## Required packages

PyTorch 
midiutil
einops
sklearn
pandas
numpy
matplotlib
scipy
tqdm

## Neural network architectures

### Translator  

![image](https://user-images.githubusercontent.com/101393859/212066186-02d6230a-a0e0-4568-9a9b-edd4172c8a01.png | width=100)

### Discriminator

![image](https://user-images.githubusercontent.com/101393859/212066285-b053d6dd-2d9c-4b0a-9bac-fdaa82f8eb13.png | width=100)


