#Wiener G-functional expressions
Given a system with an input/output pair $(x(t),y(t))$ where the input is white noise with zero mean value and power A, we can write the output of the system as sum of a series of Wiener G-functional
$ y(n) = \sum_p (G_p x)(n)$


In the following the expressions of the G-functional up to the fifth order will be given:

$(G_0 x)(n) = k_0  = E\left\{ y(n) \right\}$ 


$(G_1 x)(n) = \sum_{\tau _1  = 0}^{N_1  - 1} k_1 (\tau _1 )x(n - \tau _1 )$



$(G_2 x)(n) = \sum_{\tau _1, \tau_2 = 0}^{N_2  - 1} k_2(\tau _1 ,\tau _2 )x(n - \tau _1 )x(n - \tau _2) - A\sum_{\tau _1  = 0}^{N_2  - 1} k_2 (\tau _1 ,\tau _1 )$


$(G_3 x)(n) = \sum_{\tau _1,\ldots,\tau_3  = 0}^{N_3  - 1} k_3 (\tau _1 ,\tau _2 ,\tau _3 ) x(n - \tau _1 )x(n - \tau _2)x(n - \tau _3)- 3A \sum_{\tau _1  = 0}^{N_3  - 1} \sum_{\tau _2  = 0}^{N_3  - 1}k_3 (\tau _1 ,\tau _2 ,\tau _2 ) x(n - \tau _1 )$


$\begin{aligned}
(G_4 x)(n) = {} &  \sum_{\tau_1,\ldots,\tau_4  = 0}^{N_4  - 1} k_4 (\tau_1 ,\tau_2 ,\tau_3 ,\tau_4 )
 x(n - \tau_1 )x(n - \tau_2 )x(n - \tau_3 )x(n - \tau_4 )  + {} \\[6pt]
& {} - 6A \sum_{\tau _1,\tau _2 = 0}^{N_4  - 1} \sum_{\tau_3 = 0}^{N_4  - 1} k_4 (\tau_1, \tau_2, \tau_3 ,\tau_3) x(n - \tau_1 )x(n - \tau_2) + 3A^2 \sum_{\tau_1,\tau_2  = 0}^{N_4  - 1} k_4 (\tau_1 ,\tau_1 ,\tau_2 ,\tau_2 )    
\end{aligned}$




$\begin{aligned}
(G_5 x)(n) = {} & \sum_{\tau _1,\ldots,\tau _5  = 0}^{N_5  - 1} k_5 (\tau_1, \tau_2, \tau_3, \tau_4, \tau_5 )
 x(n - \tau_1 )x(n - \tau_2 )x(n - \tau_3 )x(n - \tau_4 )x(n - \tau_5 ) + {} \\[6pt]
& {} - 10A\sum_{\tau _1,\ldots,\tau _3  = 0}^{N_5  - 1} \sum_{\tau _4  = 0}^{N_5  - 1} k_5 (\tau_1, \tau _2 ,\tau_3, \tau_4, \tau_4 ) x(n - \tau_1 )x(n - \tau_2 )x(n - \tau_3 ) \\[6pt]
& {} + 15A^2 \sum_{\tau _1  = 0}^{N_5  - 1} \sum_{\tau_2,\tau_3  = 0}^{N_5  - 1} k_5 (\tau_1, \tau_2, \tau_2 ,\tau_3 ,\tau_3 ) x(n - \tau_1 ).
\end{aligned}$
