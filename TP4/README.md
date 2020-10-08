# ROB 311 class project - TP4

The associated code, \href{https://github.com/PPatrickGU/ROB311/blob/master/TP4/TP4_SVM.ipynb}{TP4 SVM: support vector machines} is constituted by three parts: a simple implementation of PCA and SVM, an implementation with $make\_pipeline$ and finally a try with the $Grid\_search$. The results can also be found in the repository of GitHub.

In $Pipeline$ we ensemble all the models needed and make them into one entity to have a clearer architecture of the models. In this way all the models can also be trained together.

$Grid\_search$ is a method to find the best parameters. Before training, all the hyper-parameters are given in the grid, and the best models will be found during the training. In our code, the parameter $\textbf{C}$ and different kernel choices are given for the $Grid\_search$.

\begin{itemize}
    \item[1)] $\textbf{C}$: The C parameter tells the SVM optimization how much we want to avoid misclassifying each training example. For large values of C (Lower bias, high variance), the optimization will choose a smaller margin hyperplane. A very small value of C (higher bias, low variance) will cause the optimizer to look for a larger-margin separating hyperplane, even if that hyperplane misclassifies more points.
    
    \item[2)] $\textbf{Kernel}$: The function of the kernel function is mapping from low-dimensional space to high-dimensional space. Two types of linearly inseparable points in the low-dimensional space can be turned into linearly separable in the high-dimensional space. Using ‘linear’ will use a linear hyperplane (a line in the case of 2D data). ‘rbf’ and ‘poly’ uses a non linear hyper-plane.
\end{itemize}
