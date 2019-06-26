# Complex Network Analysis with Instagram Data

This project implements the creation and visualization of a Complex Network of hashtags (also refered here as tags) on Instagram posts about politics in Brazil. An article about it at Medium.com is available [here](XXX).

The project works with some concepts about the process of data collection and construction, handling and visualization of Graphs.

Jupyter Notebook is required to collect and analyse the data. [Gephi](https://gephi.org/) is required to open, handle and visualize the graphs (and it requires Java).

## Contents

This section describes the contents in the repository.

### Notebooks

- **2019-06-10-1-macj-instagram-tags.ipynb**: designs and tests of functions to collect data from Instagram

- **2019-06-10-2-macj-collecting-data.ipynb**: performing data collection and saving to JSON file

- **2019-06-11-1-macj-graph-scratch.ipynb**: analysing the data, creating and exporting graphs

The data collected on 2019-06-11 is saved to the file `data.json`.

### GraphML Files

The GraphML files represents the networks generated.

The number in the files means the number of posts in the analysis (must be changed in future works).

- **edges\_counted\_100.graphml**: graph with edges between all tags without node weight

- **edges\_counted\_100\_dropped.graphml**: graph with insignificant edges dropped

- **edges\_counted\_keys\_100.graphml**: graph with edges between key tags and all others without node weight

- **edges\_counted\_100\_nw.graphml**: graph with edges between all tags with node weight

- **edges\_counted\_100\_dropped\_nw.graphml**: graph with insignificant edges dropped

- **edges\_counted\_keys\_100\_nw.graphml**: graph with edges between key tags and all others with node weight

All these files can be opened directly in Gephi to perform other analysis.

### Gephi Files

Gephi files contains the networks with filters, colors, scales and layouts applyied.

Bellow are short descriptions for each one.

_The following views use GraphML files without node weights:_

* v01-all-edges.gephi

  - Workspace 3: original imported network

  - Workspace 6: Force Atlas 2 layout

  - Workspace 7: Force Atlas 2 layout

* v02-key-edges.gephi

	- TODO

* v03-key-edges-fruchterman.gephi

  - Workspace 2: Fruchterman layout

_The following views use GraphML with node weights:_

* v04-key-edges-node-weight.gephi

	- TODO

* v05-all-edges-node-weight.gephi

  - Workspace 1: Fruchterman layout with Expansion and Adjust Label

  - Workspace 3: Force Atlas layout

  - Workspace 4: Force Atlas 2 layout

  - Workspace 5: Fruchterman layout for long time

  - Workspace 6: original imported network
