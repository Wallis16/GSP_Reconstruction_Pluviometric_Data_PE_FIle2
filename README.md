# GSP_Reconstruction_Pluviometric_Data_PE
GSP reconstruction from a smooth signal about pluviometric data from a state in Brazil.
First at all I get data from measurement stations (http://www.apac.pe.gov.br/) in PE (state from Brazil). 
So sampling the signal removing 37 stations, these stations were defined by me. You can see highlights showing the 37 nodes 
in image_estimated.

Solving a optimizing problem (arg min ||Ls||l2, L is the Laplacian and s is the signal, 37 unknown values and the others are fixed)
we want to estimate the values in the 37 removed nodes. Must be clear that the 37 nodes are the variables that will be estimated.
Our signal is smooth and we do not know about the bandwith length.  

There are many considerations and we can get different results just modifying the adjacency matrix. My next goal is develop a code 
that can reconstruct signals more precisely and considering more parameters.
