# Minimal Cookie Cutter Template for Data Science Projects

This is our suggested minimal structure for a data
science project.

To use this, you will need to use the `cookiecutter` tool. Which
can be installed either through conda:

`conda install cookiecutter`

Or can be installed through pip:

`pip install cookiecutter`

To create a new project, you can then use 
the command:

`cookiecutter https://github.com/l-gorman/minimal-ds-proj`

You will be asked to fill in the following values

```
    directory_name [Name of the folder for the project]: 
    year [Year the project was created]: 
    authors [Name of the author(s) involved in the project]: 
    shared_library_code [Name of shared library (package) you will develop for this project]: 
```

This will create a project with the following structure:

```
DIRECTORY_NAME/
├── README.md
├── .gitignore
├── LICENSE.md
│
├── data
|   ├── private_data 
│   │   ├── external
│   │   ├── interim
│   │   ├── processed
│   │   └── raw
│   └── public_data
│
├── docs
├── notebooks
├── outputs
├── tests
└── utils 
```

## Our recommendations
Feel free to use other frameworks. We recommend
the following:

- Documentation: https://www.mkdocs.org/
- Virtual Environments (Python): Conda
- R environments: Renv
...


## Things to Note

* We suggest functions you develop should be stored in a shared library that can be imported
* The default license is MIT license.
* By default, this project will ignore any files stored in the private data folder. Data you intend to share via github can be included in the public folder, though we would recommend this is only used for example data



