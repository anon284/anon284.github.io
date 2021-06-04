# Diffusion Schr&ouml;dinger Bridge with Applications to Score-Based Generative Modeling

This repository contains the implementation for the paper Diffusion
Schr&ouml;dinger Bridge with Applications to Score-Based Generative Modeling.

Contributors
------------

* ???

What is a Schr&ouml;dinger bridge?
-----------------------------

The Schr&ouml;dinger Bridge (SB) problem is a classical problem appearing in
applied mathematics, optimal control and probability; see [1, 2, 3].  In the
discrete-time setting, it takes the following (dynamic) form. Consider as
reference density p(x<sub>0:N</sub>) describing the process adding noise to the
data.  We aim to find p\*(x<sub>0:N</sub>) such that p\*(x<sub>0</sub>) =
p<sub>data</sub>(x<sub>0</sub>) and p\*(x<sub>N</sub>) =
p<sub>prior</sub>(x<sub>N</sub>) and minimize the Kullback-Leibler divergence
between p\* and p. In this work we introduce **Diffusion Schrodinger Bridge**
(DSB), a new algorithm which uses score-matching approaches [4] to
approximate the *Iterative Proportional Fitting* algorithm, an iterative method
to find the solutions of the SB problem. DSB can be seen as a refinement of
existing score-based generative modeling methods [5, 6].


![Schrodinger bridge](schrodinger_bridge.png)

Code
------------

Code available [here](https://github.com/anon284/schrodinger_bridge)



Two dimensional examples
------------------------

<p float="left">
  <img src="gif/circle_init.png" width="300" />
  <img src="gif_schro/circle_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/moon_init.png" width="300" />
  <img src="gif_schro/moon_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/pinwheel_init.png" width="300" />
  <img src="gif_schro/pinwheel_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/mixture_init.png" width="300" />
  <img src="gif_schro/mixture_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/swiss_init.png" width="300" />
  <img src="gif_schro/swiss_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/scurve_init.png" width="300" />
  <img src="gif_schro/scurve_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/8gaussians_init.png" width="300" />
  <img src="gif_schro/8gaussians_0123.gif" width="300" /> 
</p>

<p float="left">
  <img src="gif/checker_init.png" width="300" />
  <img src="gif_schro/checker_0123.gif" width="300" /> 
</p>

CelebA example
--------------

![celeba](gif/celeba.gif)

MNIST example
--------------

![MNIST](gif/mnist_out.gif)


Dataset interpolation
--------------

<p float="left">
  <img src="gif/moon_init.png" width="235" />
  <img src="gif_interpolation/moon2scurve.gif" width="235" />
  <img src="gif/scurve_init.png" width="235" />
</p>

<p float="left">
  <img src="gif/scurve_init.png" width="235" />
  <img src="gif_interpolation/scurve2moon.gif" width="235" />
  <img src="gif/moon_init.png" width="235" />
</p>

<p float="left">
  <img src="gif/circle_init.png" width="235" />
  <img src="gif_interpolation/circle2scurve.gif" width="235" />
  <img src="gif/scurve_init.png" width="235" />
</p>



References
----------

.. [1] Hans F&ouml;llmer
       *Random fields and diffusion processes*
       In: École d'été de Probabilités de Saint-Flour 1985-1987

.. [2] Christian Léonard 
       *A survey of the Schr&ouml;dinger problem and some of its connections with optimal transport*
       In: Discrete & Continuous Dynamical Systems-A 2014

.. [3] Yongxin Chen, Tryphon Georgiou and Michele Pavon
       *Optimal Transport in Systems and Control*
       In: Annual Review of Control, Robotics, and Autonomous Systems 2020

.. [4] Aapo Hyv&auml;rinen and Peter Dayan
       *Estimation of non-normalized statistical models by score matching*
       In: Journal of Machine Learning Research 2005

.. [5] Yang Song and Stefano Ermon
       *Generative modeling by estimating gradients of the data distribution*
       In: Advances in Neural Information Processing Systems 2019

.. [6] Jonathan Ho, Ajay Jain and Pieter Abbeel
       *Denoising diffusion probabilistic models*
       In: Advances in Neural Information Processing Systems 2020
