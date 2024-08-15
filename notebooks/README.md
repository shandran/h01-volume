# H01 visualization tools

***

# Contents

## Jupyter Notebook files

Use [`h01_plotly_visualizer.ipynb` notebook](https://github.com/shandran/h01-volume/blob/main/notebooks/h01_plotly_visualizer.ipynb) to generate a 2D and 3D interactive views of one or more cells of interest from the H01 volume. Uses matplotlib and plotly visualization methods. See an example visualization below. Note that many cell meshes are enormous (1 GB) and may cause memory allocation issues on typical computer systems.

![plotly visualization of neurons and glia in H01 volume](img/h01_plotly_screenshot.png "plotly visualization of neurons and glia in H01 volume")

Use [`pyvista_decimate_mesh_astro_cell_bodies_h01.ipynb`](https://github.com/shandran/h01-volume/blob/main/notebooks/pyvista_decimate_mesh_astro_cell_bodies_h01.ipynb) to decimate meshes (default setting is 95%) of any cell meshes that you downloaded using the `h01_plotly_visualizer.ipynb` notebook. Note that large astrocytes can take multiple hours to decimate (up to 12+ hours), whereas less complex astrocytes and neurons typically take minutes to decimate on a typical laptop.

Use [`vtk_decimated_astro_meshes_h01.ipynb`](https://github.com/shandran/h01-volume/blob/main/notebooks/vtk_decimated_astro_meshes_h01.ipynb) to generate a 3D interactive render of decimated meshes using vtk and OpenGL viewer. There are a variety of rendering methods that help bring out more clarity of the astrocyte cell membrane, including gradient coloring and opacity settings. Use matplotlib colormaps to change color settings and modify the opacity levels, camera view settings, and gradient method (linear or exponential).

![one blood vessel and two astrocytes rendered using  gradient color and opacity](img/astros_58293602559_49297401554_5101516913_2024_08_15_1504_32.png "one blood vessel and two astrocytes rendered using  gradient color and opacity")
