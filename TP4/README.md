# ROB 311 class project - TP4

The associated code is constituted by three parts: a simple implementation of PCA and SVM, an implementation withmake_pipelineand finally a try with the *Grid_search*. 

In Pipeline we ensemble all the models needed and make them into one entity  to have a clearer architecture of the models. In this way all the models can also be trainedtogether. *Grid_search* is a method to find the best parameters. Before training, all the hyper-parameters are given in the grid, and the best models will be found during the training. 

In our code, the parameter ***C*** and different ***Kernel*** choices are given for the *Grid_search*.


1) ***C***: The C parameter tells the SVM optimization how much we want to avoid misclassifying each training example. For large values of C (Lower bias, highvariance), the optimization will choose a smaller margin hyperplane. A very smallvalue of C (higher bias, low variance) will cause the optimizer to look for a larger-margin separating hyperplane, even if that hyperplane misclassifies more points.


2) ***Kernel***: The function of the kernel function is mapping from low-dimensional space to high-dimensional space. Two types of linearly inseparable points in thelow-dimensional space can be turned into linearly separable in the high-dimensionalspace. Using ‘linear’ will use a linear hyperplane (a line in the case of 2D data).‘rbf’ and ‘poly’ uses a non linear hyper-plane.
