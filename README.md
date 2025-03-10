# Analysis of myelin traces in THG images of cerebellum folia

Two stages of folium development were acquired by THG imaging:
- Beginning of myelination (DIV4)
- Peak of myelination (DIV6)

The myelin fibers and the trunk outliers from the two stages were traced manually using Imaris software. Then, the fibers morphologies relatively to the trunk outliers were measured using GeNePy3D [].

## Data

The myelin traces (.ims files) and the surfaces of trunk outliers (.stl files) were found in the folder data.

## The notebook process_data.ipynb

This notebook imported the traced myelin and the surface of trunk outlier, compute the intersections between fibers and trunk outlier and measure the number of intersected fibers, their lengths, their orientations and their tortuosities. The output is saved in df.csv in folder output.

## The notebook quantify_data.ipynb

This notebook quantified the fiber features obtained from the process_data.ipynb.

## Running the notebooks



