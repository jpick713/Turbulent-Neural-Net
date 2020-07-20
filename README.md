# Turbulent-Neural-Net
Recurrent Neural Network for predicting anisotropic stress tensor
The ground truth data is pulled from JHUTDB database with a simple jupyter lab script, and the network has two parts. 

1) A physics-embedding autoencoder which not only encodes the data for ease of training later on, but also encodes the vector potential and no slip boundary conditions, thereby ensuring zero divergence and non-slip boundary conditions.

2) A 3d temporal variant of TBNN is trained on the encoded data. 
