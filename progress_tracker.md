# MNIST Interpretability Progress Tracker

## Project Overview

The project consists of two parts. 

### Part 1: Training the Simplenet CNN Model on MNIST

- [X] Import and tweak the model for the MNIST task from the Github repo
- [X] Write training and evaluation loops for Simplenet CNN model

### Part 2: Visualization and Interpretability

- [X] Implement guided backpropagation for visualization
- [X] Visualize the learning patterns of the model on misclassified samples
- [X] Generate attention maps using guided backpropagation for specific layers and feature maps in the CNN
- [X] Using Pytorch libraries generated visual graphs of the SimpleNet model
 
## Milestones

### Milestone 1: Part 1 Completion

- [X] Complete training and evaluation loops for Simplenet CNN model
- [X] Successfully import and tweak the model for the MNIST task
- [X] Train the model on the MNIST dataset

### Milestone 2: Part 2 Completion

- [X] Implement guided backpropagation for visualization purposes
- [X] Visualize the learning process of the model on misclassified samples
- [X] Generate attention maps using guided backpropagation for specific layers in the CNN

## Next Steps

- [ ] Read about and apply the pruning technique in order to optimize learning 
- [ ] Visualize the modified learning behaviour with gbp (layerwise) attention maps
- [ ] Retrain the model


## Notes and Updates

- Every result is saved on jupyterhub, because for training I'm using a jupyter remote virtual environment on VM
- I prefer to use VSCode as IDE for debugging and ease of use, and it works with minor tweaks to the repo, but I also need to clone it locally to work with local variables (in the VSCode jupyter notebook) 
- Using torchview and torchviz requires downloading the local files of the graphviz parent library and do a path append to the bin dir, so for that part I switched to the "mytorch" local conda environment, with minor changes to the code (use of src.models prefix when importing the simplenet models scripts) 
- 

## References and Resources 

- Repositories used: 
    - SimpleNet: https://github.com/Coderx7/SimpleNet_Pytorch
    - CNN Visualizations (with guided backpropagation): https://github.com/utkuozbulak/pytorch-cnn-visualizations

- Software libraries for Visualizarion:
    - Torchview
    - Torchviz 
    - Netron (appears to be the best)

- CNN Visualization: 
    - Visualizing and Understanding CNNs by Zeiler et al: https://arxiv.org/abs/1311.2901
    - https://youtu.be/eASwKmKYWeo?si=YDPCRd4F-2WZEChA
    
- Pruning: 
    - Introductory paper from '87: file:///C:/Users/iustin.grigoras/Downloads/Hanson-Pratt.pdf
    - Deep Compression: Compressing Deep NNs with Pruning, Trained Quantization and Hoffman Coding - ICLR 2016: https://arxiv.org/pdf/1510.00149.pdf
    - Medium blogpost: https://olegpolivin.medium.com/experiments-in-neural-network-pruning-in-pytorch-c18d5b771d6d