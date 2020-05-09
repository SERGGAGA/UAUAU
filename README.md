I write
import matplolib.pyplot as plt
import numpy as np
import sympy as smp

d, ro=smp.symbols('d ro')

n=1.6#refracive index
angle=6*np.pi/180#angle
R=5#sm sheric mirror
c=10#sm lenght do pertyagka
d=1#sm lenght of cristall



cavity_mat=smp.Matrix([[1, d], [0, 1]])
smooth_mirror_mat=smp.Matrix([[1, 0], [0, -1]])
sheric_mirror_mat=smp.matrix([[1, 0], [-2/(R*np.cos(angle)), 0]])
a=np.arange(0, 100)
