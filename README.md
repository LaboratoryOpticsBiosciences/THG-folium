# Analysis of myelin traces in THG images of cerebellum folia

Two stages of folium development were acquired by THG imaging:
- Beginning of myelination (DIV4)
- Peak of myelination (DIV6)

The myelin fibers and the trunk outliers from the two stages were traced manually using Imaris software. Then, the fibers morphologies relatively to the trunk outliers were measured using [GeNePy3D](https://genepy3d.gitlab.io/).

## Data

The myelin traces (.ims files) and the surfaces of trunk outliers (.stl files) are found in the folder *data*.

## The notebook process_data.ipynb

This notebook imports the traced myelin and the surface of trunk outlier, computes the intersections between fibers and trunk outlier and measures the number of intersected fibers, their lengths, their orientations and their tortuosities. The output is saved in df.csv in folder *output*.

## The notebook quantify_data.ipynb

This notebook quantifies the fiber features obtained from the process_data.ipynb. 

## Running the notebooks

The notebooks were run in python 3.9 with some dependencies. Below is the installation using conda.


```
conda create -n "thg-folium" python=3.9
conda activate thg-folium
pip install -U genepy3d genepy3d_gpl notebook
```

Additionally, CGAL-SWIG must be installed, see [this](https://genepy3d.gitlab.io/install_cgal_swig_ubuntu) for installation detail.
