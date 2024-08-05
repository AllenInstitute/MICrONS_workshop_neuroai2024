# MICrONS workshop for NeuroAI Conference, 8 August 2024

Offered in participation with the Neuroscience and Artificial Intelligence Conference at the University of Washington. [See conference program and details here](https://www.neuroaiseattle.com/))

![neuro-ai](https://github.com/user-attachments/assets/2e41f315-9db4-4099-b53d-16c5d2b092be)

## MICrONS dataset tutorial: Functional connectomics spanning multiple areas of mouse visual cortex
Presented by Bethanny Danskin and Casey Schneider-Mizell, with material from Sven Dorkenwald and Forrest Collman.

The MICrONS dataset is a large functional connectomics dataset with dense calcium imaging and electron microscopy based cell reconstruction of a millimeter scale volume. All neurons were automatically reconstructed and all synapses detected. Subsequent proofreading in this volume yielded reconstructions that include complete dendritic trees for all ~70 thousand neurons as well the local and inter-areal axonal projections of a subset of neurons that map up to thousands of cell-to-cell connections per neuron. Functional measurements and connectivity can be related for ~12 thousand neurons which were coregistered between the calcium and EM volumes. In this tutorial, we introduce the dataset, as well as both interactive and programmatic tools to analyze it. The tutorial will contain exercises for hands on work and time to explore the dataset on your own laptop.   

Manuscript describing the dataset: https://www.biorxiv.org/content/10.1101/2021.07.28.454025v3.abstract

### Dataset introduction

slides: https://docs.google.com/presentation/d/1gEOZAE9B-IlOkxbOEulgOgTp0XWfhbtk__Ve3Cjvc64/edit?usp=sharing

cell type model paper: https://www.biorxiv.org/content/10.1101/2022.07.20.499976v2

dataset paper: https://www.biorxiv.org/content/10.1101/2021.07.28.454025v3

inhibitory connectivity paper: https://www.biorxiv.org/content/10.1101/2023.01.23.525290v3

CAVE: https://www.biorxiv.org/content/10.1101/2023.07.26.550598v1

### Neuroglancer: data visualization and exploration

Launch the viewer with preselected interesting states from the [MICrONs-Explorer Gallery page](https://www.microns-explorer.org/gallery-mm3 ).

Launch a [neuroglancer viewer](https://neuroglancer.neuvue.io/?json_url=https://global.daf-apis.com/nglstate/api/v1/5773646117208064) of the updated public dataset.

Launch a [beta] [spelunker neuroglancer viewer](https://spelunker.cave-explorer.org/#!middleauth+https://global.daf-apis.com/nglstate/api/v1/4954638937751552) of the updated public dataset.

### DashApps: interactive online analysis

Browse the data tables, including cell type classifications with the [Table Viewer](https://minnie.microns-daf.com/dash/datastack/minnie65_public/apps/table_viewer/?datastack=%22minnie65_public%22).

Query and visualzie the synaptic connectivity of neurons with the [Connectivity Viewer](https://minnie.microns-daf.com/dash/datastack/minnie65_public/apps/connectivity/?anno-id=%22%22&id-type=%22root_id%22&mat-version=943&cell-type-table-dropdown=%22%22&datastack=%22minnie65_public%22)

### Programmatic Access: using the Connectome Annotation Versioning Engine (CAVE) ecosystem

Follow the tutorial for [setup and quickstart here](https://github.com/sdorkenw/MICrONS_workshop/blob/main/tutorials/ProgrammaticAccess.ipynb )

There are two options for following the tutorial and doing the exercises:
1. Local: [Create a new conda environment](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands) using Python 3.11 (specificall not 3.12!) and `pip install caveclient` into it as well as your favorite notebook package (e.g. `pip install jupyter`).
2. Online: Head over to [colab.research.google](https://colab.research.google.com/github/AllenInstitute/MICrONS_workshop_neuroai2024/blob/main/tutorials/ProgrammaticAccess.ipynb)  requires GMail or GMail-enable account). On the left side select "GitHub" and paste in the link to the notebook on github.

### Dataset documentation

More complete documentation that includes the above information as well as guides to interacting with meshes, skeletons, and imagery, [can be found online](https://alleninstitute.github.io/microns_tutorial/).
