# Robust Self-Attention Deep Generative Model for Anomaly Detection in Industrial Cyber-Physical Systems
Cyber-physical systems (CPSs) have attracted increasing attention in recent years due to their promise of substantial and long-term benefits to society, the economy, the environment, and citizens. In addition, the rapid advances in computing, communication, and storage technologies have revolutionized the information communication technology domain and domination in the industry context. Using CPSs in industrial settings has led to industrial cyber-physical systems (ICPSs), which enable large-scale cooperation in industrial facilities and among all the value chain stakeholders in conjunction with information-driven interactions. ICPSs are widely used and vital to industry and society. Their failure can have a severe impact on both the economy and human life. Hence, these systems have become an attractive target for physical and cyber-attacks. Deep generative models have demonstrated their effectiveness in learning latent representation and modeling complex dependencies of time series. Thus, this study introduces a  novel unsupervised anomaly detection framework for complex multi-process ICPSs with various sensors and actuators. The main element of the devised methodology is a self-attention-enabled Deep Variational Convolutional Recurrent Autoencoder (Sa-DVCRAE) that relies on modeling the inter-correlations between different pairs of time series to perform robust anomaly detection. Sa-DVCRAE is based on the Variational Auto-Encoder (VAE) architecture, and its component neural networks (i.e., encoder and decoder) are assembled using convolutional and recurrent layers to capture both the spatial and the temporal dependencies in the sequential data constructed from the raw time series. To further improve the reconstruction accuracy and enhance the representative power of the network, we incorporate the self-attention memory module into the ConvLSTM layers to efficiently capture the \emph{long-range} spatiotemporal patterns present in the data. Extensive experiments on three real-world datasets demonstrate that Sa-DVCRAE can outperform state-of-the-art baseline methods.

## Table Of Contents
-  [In Details](#in-details)
-  [Contributing](#contributing)
-  [Acknowledgments](#acknowledgments)
- [License](#license)

## In Details
- DoVaeSupplementary: this file contains the class Sampling, class VAE and class EarlyStoppingAtMinLoss for implementing a VAE model.
- DoSupplementaryTrain.py: diferentes métodos para guardar información cuando se ejecuta el entrenamiento del modelo.
- DoSplitData.py: data prepatation and split data.
- CBAM_attention3D.py: this file contains the class channel attention, class spatial attention for implementation of 3D-CBAM.
- 3Da-CVAE.ipynb: model 3-dimensional Attention-Based Convolutional Variational Autoencoder.

## Contributing
Any kind of enhancement or contribution is welcomed.

## Acknowledgments
The authors would like to thank iTrust, Center for Research in Cyber Security, Singapore University of Technology and Design for providing the SWaT dataset.


## License
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](https://github.com/mmacas11/3Da-CVAE/blob/main/LICENSE)**



