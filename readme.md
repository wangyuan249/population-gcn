Graph CNNs for population graphs: classification of the ABIDE dataset
---------------------------------------------------------------------

 This code provides a python - Tensorflow implementation of graph convolutional networks (GCNs) for semi-supervised 
 disease prediction using population graphs, as described in: 
 
Parisot, S., Ktena, S. I., Ferrante, E., Lee, M., Moreno, R. G., Glocker, B., & Rueckert, D. (2017). <br />
[Spectral Graph Convolutions for Population-based Disease Prediction](https://arxiv.org/abs/1703.03020). <br />
arXiv preprint arXiv:1703.03020.

We provide an implementation applied to the [ABIDE dataset](preprocessed-connectomes-project.org/abide) 
for diagnosis of Autism Spectrum Disorder.

#### INSTALLATION

To run the programme, you will need to install the implementation of graph convolutional networks (GCN) by Kipf et al.
This project is only compatible with our [forked GCN project](https://github.com/parisots/gcn).  

The root folder in fetch_data.py (line 12) and ABIDEParser.py (line 17) has to be updated to the folder were the data will be stored. 

Next, to install, organise and pre-process the ABIDE database:
python fetch_data.py 



#### USAGE

To run the programme with default parameters: 
 ```python
python main_ABIDE.py 
```
 
To get a detailed description of parameters:
 ```python
python main_ABIDE.py --help 
 ```


#### REQUIREMENTS 

tensorflow (>0.12) <br />
networkx <br />
nilearn <br />
scikit-learn <br />
joblib

#### REFERENCE 

Please cite our paper if you use this code in your own work:

```
@article{parisot2017spectral, 
  title={Spectral Graph Convolutions on Population Graphs for Disease Prediction}, 
  author={Parisot, Sarah and Ktena, Sofia Ira and Ferrante, Enzo and Lee, Matthew and Moreno, Ricardo Guerrerro and Glocker, Ben and Rueckert, Daniel}, 
  journal={arXiv preprint arXiv:1703.03020}, 
  year={2017} 
}
```



