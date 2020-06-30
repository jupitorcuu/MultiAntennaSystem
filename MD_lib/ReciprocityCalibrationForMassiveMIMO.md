#Reciprocity Calibration
## Signal Models
Uplink and downlink signal model 

   pilot signal for k users $p=diag\{p_1,p_2,\dots,p_k\}$ , $y_{UP}$ is uplink received signal $R_B$ is HW impairment model of M receivers on basestation $R_B=diag\{r_1^B,r_2^B,\dots,r_M^B\}$ , $t_U$ is HW impairment model of k transmitter from UE $t_U=diag\{t_1^U,t_2^U,\dots,t_k^U\}$  $H_p$ is propagation channel matrix, $H_{UP}$ is uplink radio channel, w is uplink noise.
   $y_{UP}=H_{UP}p+w = R_BH_pt_Up+w$
   $y_{DL}=H_{DL}z'+w'=R_UH_P^TT_Bz'+w$
   $R_U=diag\{r_1^U,r_2^U,\dots,r_k^U\}$ is HW response if receive RF chains of K users , $T_B=diag\{t_1^B,t_2^B,\dots,t_M^B\}$ is HW response of transmitter RF chains of basestation, $z'=Px$, z' is a vector with linearly precoding QAM symbols, P is precoding matrix, and x is QAM symbols.

## Calibration Coefficients 
A is Basestation, B is UE
![](Reciprocity%20model.png)

$G(t,f) = R_Be^{j2\pi f'_Bt}C(t,f)T_Ae^{-j2\pi f_At} $
$H(t,f) = R_Ae^{j2\pi f'_At}C(t,f)^TT_Be^{-j2\pi f_Bt} $
$(G(t)e^{-j2\pi(f_A-f'_B)t}) = {P_B}^{-1}(H(t)^TP_Ae^{-j2\pi(f_B-f'_A)t})$
$G(t)={P_B}^{-1}H(t)^TP_A$
$(\hat{P_A},\hat{P_B})=\argmin{\sum{\vert{\vert{P_B(\hat{G}(ti)+\tilde{G}_i)-(\hat{H}(t_i)+\tilde{H}_i)^TP_A\vert{}\vert}^2_2}}+\vert{}\vert{}\tilde{G}_i\vert{}\vert{}^2_2+\vert{}\vert{}\tilde{H}_i\vert{}\vert{}^2_2} $
