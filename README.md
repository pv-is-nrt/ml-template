# ML Template repository

Hi! This is a template repository for a machine learning study. A study is comprised of several experiments. Even if you can think of only one study for the project you have in mind, I strongly suggest you consider organizing your project in a way that allows for multiple studies.

The rough directory structure of the repo is shown below:

- packages
  although most packages should be put in the `pvnrt` repository, some niche, project-specific packages can be put here. A package is simply a collection of python files containing reusable, and importable, classes and functions.
  - \_\_init__.py (used to identify this folder as a recognizable python package)
  - plot.py
  - images.py
- data
  make sure to delete temporary and no-more-to-be-used data files, move useful but not current data files to `archive`, and keep a copy of downloaded files in the `downloaded` folder.
  - downloaded
  - archived
  - datasets
    - ds01
    - ds02
  - file1.csv
  - file2.csv
  - file3.xlsx
  - any other curated data files in use
- studies
  it is advisable to nest your experiments within a study.
  - study01
    - experiments
      - exp1
      - exp2
      - and so on
  - study02
- notebooks
  a place to keep all Jupyter notebooks. These will be used to create datasets, run experiments, make plots etc.
  - run an experiment.ipynb
  - create a dataset.ipynb
  - create a model architecture.ipynb
  - visualizations.ipynb
- notebooks (in progress)
  a place for notebooks in development
- models
  store all model architectures here. Trained models should be stored in their respective `experiment` folder.
  - FC-6-32-64-32-3-relu.json
  - CNN-500p-3L-2C-sigmoid.json
- temp
  any temporary files that will be deleted periodically.