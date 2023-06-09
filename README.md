# CS6208_GNN_paper_review
This code re-implementation the idea of Weisfeiler - Lehman Graph Kernal in python [[1]](#1)

- Adding the verbose optional which can see the change of each label graph in 1st iterator. 
![image](https://user-images.githubusercontent.com/16068098/230894187-398890cc-6352-4f0f-a6f8-1d2ded2f14af.png)
In the notebook:
   - WL_General: computes the Weisfeiler-Lehman subtree kernel
   - WL_Edge: computes the Weisfeiler-Lehman edge kernel
   - WLsp_kernel: computes the Weisfeiler-Lehman shortest path kernel (with 
exact matching of shortest path lengths)
   - RGkernel: Ramon and Gaertner subtree kernel
- We build the simple graph classification using these kernel compared to random walk kernel of GraKel library [[2]](#2) 
The result show that the computational cost of WL kernel is similar but the time to performance of WL kernel is faster  

The original paper implement these code on MATLAB. You can find the original code here [[3]](#3).

## References 
<a id = "1">[1]</a>
N. Shervashidze, P. Schweitzer, E. J. van Leeuwen,
K. Mehlhorn, and K. M. Borgwardt, Weisfeiler-
lehman graph kernels, J. Mach. Learn. Res. 12,
2539–2561 (2011), ISSN 1532-4435. </br>
<a id= "2">[2]</a> G. Siglidis, G. Nikolentzos, S. Limnios, C. Giat-
sidis, K. Skianis, and M. Vazirgiannis, Grakel: A
graph kernel library in python, Journal of Machine Learning Research 21, 1 (2020). </br>
<a id= "3">[3]</a> https://github.com/SiavashCS/CompRF/tree/master/graphkernels/labeled  </br>
