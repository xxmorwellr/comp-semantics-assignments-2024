### Resources 
- WordNet  
 https://wordnet.princeton.edu/
- Pre-trained BERT Model  
https://huggingface.co/transformers/v2.9.1/quickstart.html

### Pay attention to!
- Due to the imbalanced distribution of word senses, *normalization* should be considered when comparing per word form accuary. Is the normalization method here suitable? => weighted accuracy should be weighted **not** by the number of senses, but by their *distribution* which would reflect some kind of importance.
- How to improve the performance by *enhanced data-preprocessing*? More implemental details...
