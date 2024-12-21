 We have used the software R and the libraries MittagLeffleR, kStatistics and stabledist. The code refers to the figures in Paragraph 3.1 of https://arxiv.org/pdf/2412.14979 .
 
 The first figure shows the values of $p_n(t)$ (the probability of observing $n$ events up to time $t$, starting from 0 at time 0) of the exchangeable fractional Poisson process,  
 obtained by using the analytical formula (red dots) and the corresponding simulated values (green triangles), in the case $\lambda = 1$.
 Notably, these results are essentially coinciding. For the Monte Carlo simulation, we have used 1,000,000 independent random numbers following the Lamperti distribution;
 to this aim, we used that a Lamperti random variable of parameter $\nu$ is equal in law to the ratio of two independent, positive, 
 $\nu$-stable random variables. Then we have generated the vector N, of length 1,000,000, whose j-th component 
 is a realization of a Poisson random variable of parameter $t\cdot$L[j], being L the vector which contains the realizations the Lamperti variable. 
 Finally we computed the relative frequency of the events that approximates  $p_n(t)$ for each $n$. 
 We repeated the simulation for $t = 1,2,5$ and $\nu = 0.1, 0.5, 0.9$.

The second figure shows a trajectory of the exchangeable fractional Poisson process for different values of the parameter $\nu$, up to $n = 10,000$ events. 
Here we have generated $n$ values from a Lamperti distribution of parameter $\nu$, for $\nu = 0.5, 0.75, 0.9$, as explained before, and we have saved them in a vector L. 
Then we have generated the first $n$ waiting times, each of them as a realization of an exponential distribution with parameter L[j].
Finally, the trajectory is obtained cumulating the waiting times. The waiting times become longer, as the value of $\nu$ decreases.

