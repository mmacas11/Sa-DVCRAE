# Robust Self-Attention Deep Generative Model for Anomaly Detection in Industrial Cyber-Physical Systems
Industrial Cyber-Physical Systems (ICPSs) play a crucial role in modern industries, offering numerous benefits but also becoming a prime target for physical and cyber-attacks due to their increasing complexity and integration with information technology. Deep generative models have demonstrated their effectiveness in learning latent representations and modeling the complex dependencies of time series. In this work, we strive to enhance the security of complex multi-process ICPSs incorporating various sensors and actuators by proposing a novel unsupervised anomaly detection framework built around a self-attention-enabled Deep Variational Convolutional Recurrent Autoencoder (Sa-DVCRAE). The proposed model captures temporal and spatial dependencies in the sequential correlation matrices constructed from the raw ICPS multivariate time series by employing a Variational Autoencoder (VAE) architecture with a convolutional recurrent encoder and decoder. By integrating a self-attention mechanism, the model efficiently captures long-range spatiotemporal patterns in the data, further enhancing its encoding-decoding capability. Anomaly detection is performed using the reconstruction probability, a novel approach that yields superior results compared to deterministic reconstruction errors. Additionally, we introduce a nonparametric and state-based anomaly thresholding mechanism, achieving high anomaly detection performance with low overhead. Extensive experiments on three datasets (SWaT, HAI, BATADAL) demonstrate the superior performance of Sa-DVCRAE over state-of-the-art baseline techniques. Finally, the source code of our implementation is made publicly available to promote reproducibility and encourage further research.

## Table Of Contents
-  [In Details](#in-details)
-  [Contributing](#contributing)
-  [Acknowledgments](#acknowledgments)
- [License](#license)

## In Details
- DoVaeSupplementary: this file contains the class Sampling, class VAE, and class EarlyStoppingAtMinLoss for implementing a VAE model.
- DoSupplementaryTrain.py: different methods to save information when model training is executed.
- DoSplitData.py: data preparation and split data.
- SaConvLSTM.py: this file contains a variant of the LSTM network and captures spatial features in multi-dimensional data by the convolution process. To further enhance the representation power of the model and improve reconstruction accuracy, we incorporate the self-attention memory (SaM) module into the ConvLSTM layers.
- DoModels_ML.py: it contains the self-attention-enabled Deep Variational Convolutional Recurrent Autoencoder (Sa-DVCRAE) model.
- DoMatrices.py: it allows to create the correlation matrices.

## Contributing
Any kind of enhancement or contribution is welcomed.

## Acknowledgments
- The authors thank iTrust, the Center for Research in Cyber Security, Singapore University of Technology and Design, for providing the SWaT dataset.
- Lin, Z., Li, M., Zheng, Z., Cheng, Y., & Yuan, C. (2020, April). Self-attention convlstm for spatiotemporal prediction. In Proceedings of the AAAI conference on artificial intelligence (Vol. 34, No. 07, pp. 11531-11538).

## License
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

- **[MIT license](https://github.com/mmacas11/Sa-DVCRAE/blob/main/LICENSE)**



