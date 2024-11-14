# Repository for Text Analytics project (Group 4)

## Directories
- `data`: raw data (at the moment the training and test sets for the task);
- `src`: the project source code (jupyter notebooks, scripts etc.);
- `results`: intermediate data generated during cleanup and analysis as well as final results such as figures and tables;
- `doc`: documents associated with the project, like files for manuscripts etc. (at the moment the project proposal)

Remember to name all files according to their content or function.

> [!NOTE]
> Since the embeddings database is very large, it is not tracked in the repository (neither should it be tracked since it cannot be distributed). You can dowload it from [http://www.italianlp.it/download-italian-twitter-embeddings/](http://www.italianlp.it/download-italian-twitter-embeddings/) after filling out the form and put the `.sqlite` file in the `data` directory.

## Installation
### Clone this repository

```
git clone https://github.com/g-fabiani4-unipi/txa_project.git
cd txa_project
```

### Environment and dependencies
Create an environment with your preferred method. For example with anaconda you can use:
```
conda create -n txa_project python=3.12
conda activate txa_project
```

Then install the requirements running
```
pip install -r requirements.txt
```

Remember to track newly installed software using

```
pip freeze > requirements.txt
```

### Git integration
[Nbdime](https://nbdime.readthedocs.io/en/stable/) is installed in the environment and integrated with git.
```
git diff [<commit> [<commit>]] [--] [<path>…​]
```
should give you the standard diff for non notebook files and Nbdime's diff for all `.pynb` files.

You can also launch the rich web-based tool for diff visualization with
```
nbdiff-web [<commit> [<commit>]] [<path>]
```
