# MATLABaccidents
For MATLAB accidents that lead to interesting results

Add any funny or fancy code that you got doing MATLAB stuff

---

The following accident are included:

# Bone-sets

![](/Images/bone-sets.gif)

**Author:** Ander Biguri

**Medium:** Arithmetic Bug on gif

Level-set algorithm attempting to segment a 3D volume of a CT scan of a human thorax. 
An opposite sign generates a trippy biologically looking image while still partially segmenting the bone structure.



# Mondrian.gif

![](/Images/mondrian.gif)

**Author:** Ander Biguri

**Medium:** Indexing/Arithmetic Bug on gif

A miserably failed attempt to generate projections from tetrahedra meshes. 
Error unknown. 

# Zebra Bregman

![](/Images/Zebra_bregman.png)

**Author:** Ander Biguri

**Medium:** Arithmetic Bug on png

Split-Bregman globally convex segmentation misses a sign, decides to go full sabanah horse.

# triangle_mesh_index_error

![](/Images/triangle_mesh_index_error.png)

**Author:** Ander Biguri

**Medium:** Indexing Bug on png

Triangles look very nice when plotted, but the importance of a -1 in the code can not be ignored, as this crude representation of aberrant indexing shows. 

# subgradient_descend_bye_bye

![](/Images/subgradient_descend_bye_bye.png)

**Author:** Ander Biguri

**Medium:** Mathematics on png

When the derivatives are wrong, the gradient goes to hell (or in that general direction). The solution is be in the center.

# Infiniteloop

![](/Images/infiniteloop.png)

**Author:** Ander Biguri

**Medium:** Floating point accuracy on png

Look, I needed all those decimals, and float32 was not giving me all those decimals. Decimals are what I wanted. Lots of them.

# recosntruction_index_error

![](/Images/recosntruction_index_error.png)

**Author:** Ander Biguri

**Medium:** Indexing error on png

Sometimes bad indexing just generates pretty images. Just that, just pretty images.

# covariance and covariance2

![](/Images/covariance.png)

![](/Images/covariance2.png)

**Author:** Adriaan

**Medium:** Colormaps on png

Maybe a different colormap represent better this isolines of the covariance? Maybe.

# map_of_USA

![](/Images/map_of_USA.png)

**Author:** Dev-il

**Medium:** png

USA looked different in my school maps.

# derp_cornu

![](/Images/derp_cornu.png)

**Author:** Luis Mendo

**Medium:** Too many things on png

One cornu was good, by why not just put more?

# yarn

![](/Images/Yarn.png)

**Author:** Luis Mendo

**Medium:** Too many things on png

Each line represents the complex-plane trajectory of a multipath fading process, generated as complex correlated Gaussian noise. I meant to plot the absolute value as a function of an implicit time index, i.e. `plot(abs(x))` (equivalent to `plot(1:size(x,1), abs(x))`), but I mistakenly did `plot(x)`, which draws the paths on the complex plane (and gives a prettier result).

# Nope Inverse

![](/Images/nopeInverse.png)

**Author:** flawr

**Medium:**  Wrong inverse of geometric transform on png

These lines should form a rectangular grid. Turns out the inverse I computed doesn't actually invert the original function.


# "sphere"

![](/Images/sphere.png) 
![](/Images/sphere_fixed.png)

**Author:** flawr

**Medium:** mixed sign- and off-by-one errors

The shape in the first picture is supposed to be a unit sphere. The coordinates should have been normalized by `v = v/norm(v)^1`, instead they were normalized by `v=v*norm(v)^2`. The second picture shows an attempt to fix it by doing `v = v/norm(v)^4`.

# polyhedron

![](/Images/polyhedron_no_intersection.png) 

**Author:** flawr

**Medium:** matplotlib doesn't do intersections

This was ported from MATLAB to python, but unlike MATLAB, matplotlib doesn't automatically compute intersections of 3d polygons - at least not with the method used.

