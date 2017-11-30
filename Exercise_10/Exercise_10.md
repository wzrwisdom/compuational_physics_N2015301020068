# Exercise 12---the three-body problem (the Sun & the Earth & the Jupiter) 
2015301020068 王子睿 

# 1. Abstract
A three-body system made up of the Sun, the Earth and the Jupiter is built to investigate the effect on the Earth's motion introduced by the gravitational force between the Earth and the Jupiter. The mass of the Jupiter is changed to illustrate this influence.  

# 2. Background
In the problem of celestial mechanics, three-body problem or n-body problem is much more common than two-body ones. Meanwhile, their analytical theory becomes much more complicated. Since Jupiter is the largest planet in the solar system, we consider a three-body problem consisting of the Sun, the Earth and the Jupiter. Without Jupiter, the orbit of the Earth is stable and unchanging with time.   
Besudes, we have the masses of the planets as follows:  
![](http://latex.codecogs.com/gif.latex?m_S%3D2.0%5Ctimes10%5E%7B30%7Dkg%2Cm_E%3D6.0%5Ctimes10%5E%7B24%7Dkg%2Cm_J%3D1.9%5Ctimes10%5E%7B27%7Dkg)  
![](http://latex.codecogs.com/gif.latex?x_S%3D0%2Cx_E%3D1AU%2Cm_J%3D5.2AU)  

# 3. Methodology and Solutions
## 3.1. Three-Body Problem
Generally, the magnitude of gravitational force between two planet is  
![](http://latex.codecogs.com/gif.latex?F_%7Bij%7D%3D%5Cfrac%7BGm_im_j%7D%7B%28x_i-x_j%29%5E2&plus;%28y_i-y_j%29%5E2%7D)  
The total force that the planet labeled by the subscript ![](http://latex.codecogs.com/gif.latex?i) experiences is  
![](http://latex.codecogs.com/gif.latex?%5Coverrightarrow%7BF_i%7D%3D%5Csum_%7Bj%7D%5E%7Bj%5Cneq%20i%7D%5Cfrac%7BGm_im_j%7D%7B%5Cleft%20%7C%20%5Coverrightarrow%7Br_j%7D-%5Coverrightarrow%7Br_i%7D%20%5Cright%20%7C%5E2%7D%5Ccdot%20%5Cfrac%7B%5Coverrightarrow%7Br_j%7D-%5Coverrightarrow%7Br_i%7D%7D%7B%5Cleft%20%7C%20%5Coverrightarrow%7Br_j%7D-%5Coverrightarrow%7Br_i%7D%20%5Cright%20%7C%7D)  
Here, for simplicity, we consider only three planets(the Sun, the Earth and the Jupiter). Besides, the AU is introduced to simplify the numerical process since ![](http://latex.codecogs.com/gif.latex?Gm_S%3D4%5Cpi%5E2AU%5E3/yr%5E2) and the distance ![](http://latex.codecogs.com/gif.latex?d_%7BS%2CE%7D%3D1AU).  
## 3.2 Initial Condition
For simplicity, we set the initial location of each planets as ![](http://latex.codecogs.com/gif.latex?x_S%3D0%2Cx_E%3D1AU%2Cm_J%3D5.2AU) in the rest frame.  
As for initial velocity, set it with the magnitude with which the planet circles around the Sun in a stable orbit with no extra influence.  
Because ![](http://latex.codecogs.com/gif.latex?%5Cfrac%7BGm_Sm_x%7D%7Br%5Er%7D%3Dm_x%5Cfrac%7Bv%5E2%7D%7Br%7D)  
we have ![](http://latex.codecogs.com/gif.latex?v%3D%5Csqrt%7B%5Cfrac%7BGm_S%7D%7Br%7D%7D)  

# 4. Code
Code for [the Sun is tationary](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/source1)  
Code for [the Sun is NOT stationary](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/source2)  


# 5. Running and Analysis
## 5.1 The Sun is stationary 
The mass of the Jupiter is changed so see its effect on the motion of the Earth.  The initial condition is ![](http://latex.codecogs.com/gif.latex?%5Coverrightarrow%7Br_E%7D%3D%281.%2C0.%29%2C%5Coverrightarrow%7Br_J%7D%3D%285.2%2C0.%29) and ![](http://latex.codecogs.com/gif.latex?%5Coverrightarrow%7Bv_E%7D%3D%280.%2C2%5Cpi%29%2C%5Coverrightarrow%7Bv_J%7D%3D%280.%2C2%5Cpi/%20%5Csqrt%7B5.2%7D%29)  
When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_1.png)  
The motion of the Earth is almost stable, thus it is almost not influenced.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?10m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_2.png)  
The motion of the Earth is almost stable with little procession.  The influence is small.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?100m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_3.png)  
The motion of the Earth is hardly stable and the procession is clear.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?300m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_4.png)  
The procession is clear.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?1000m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_5.png)  
The motion of the Earth is completely unstable. However, in the case of ![](http://latex.codecogs.com/gif.latex?1000m_J), the mass of the Jupiter is of the order of the Sun, so the simulation to treat the Sun stationary is not appropriate here.  

To have a clearer picture of the influence of the mass of the Jupiter on the motion of the Earth, the animation below is the trajectories of various Jupiter masses.  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/1.stationary.gif)  

## 5.2 The Sun is Not Stationary  
This is demonstrated in both the Rest Frame and the Center-of-Mass (COM) Frame.
When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_6.png)  
The motion of the system is almost stable with three planets circling around the Sun.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?20m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_7.png):  
The motion of the system is less stable. In the Rest Frame, the Earth and the Jupiter are under procession and the Sun is also moving. In the COM Frame, we can see the Sun is circling around some point.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?100m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_8.png):  
The motion of the system is hardly stable.  

When the mass of the Jupiter equals ![](http://latex.codecogs.com/gif.latex?300m_J)  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/figure_9.png) : 
The motions of each planet in the system is complicated and almost chaotic.

To grasp a deeper understanding of the Three-Body Simulation, animations are made in the Rest Frame and the COM Frame as follows. The variance of the mass of the Jupiter is marked in the figures.  
In the Rest Frame:  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/2.1restframe.gif)  
In the COM Frame:  
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/Exercise_10/2.2COMframe.gif)  

# 6. Acknowledgement and Reference
- [codecogs](http://latex.codecogs.com/)
- Computational Physics, Nicholas J. Giordano & Hisao Nakanishi

