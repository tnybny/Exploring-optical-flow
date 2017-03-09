# Optical flow

This repo explores one optical flow algorithm, namely the Lucas-Kanade method.

The optical flow problem at its most basic form makes a constant brightness assumption. That is, an object's movement in some direction causes only small change delx, dely and delt in its coordinates, while the brightness remains the same. That then leads to the famous optical flow equation f\_x u + f\_y v + f\_t = 0 where [u, v] represents optical flow in the x and y directions. This leads to an optimization problem of finding u and v. 

The method involves computation of gradients in x, y and t directions f\_x, f\_y and f\_t. An additional assumption of constant optical flow within a small 3 by 3 window centered at a pixel leads to an overdetermined system of equations. This system can then be either solved naiively by matrix operations or by minimizing errors using least squares (Lucas-Kanade). Both approaches are explored in the python notebook 'Lucas-Kanade optical flow example.ipynb'.

'Playing with image filters.ipynb' contains a small script to understand the effects of various popular image filters.

## Contact

tnybny@gmail.com
