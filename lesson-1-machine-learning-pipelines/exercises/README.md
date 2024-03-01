# Purpose of This Directory

This directory should contain any files and instructions necessary for exercises created for this lesson.

## Folder Structure

Each exercise should be contained in its own folder using the naming convention of `concept#-name-of-concept`. See example below:

```
exercises
    |_ concept1-hello-world
    |   |_ starter
    |   |   |_ exercise-files
    |   |_ solution
    |   |   |_ solution_files
    |_ concept2-foo-bar
    |   |_ starter
    |   |   |_ exercise-files
    |   |_ solution
    |   |   |_ solution_files
    |_ README.md
```

## Glossary
**Artifact:** The product of a pipeline component. It can be a file (an image, a model export, model weights, a text file...) or a directory.

**Component:** One step in a Machine Learning Pipeline. In MLflow, a component is characterized by an environment file (conda.yml if you are using conda), an entry point definition file (MLproject) and one or more scripts or commands to be executed and their supporting code.

**Container:** A technology to package together the entire runtime of a software, i.e., the code itself and all its dependencies and data files. Containers can be spun up quickly, and they run identically across different environments.

**Data Segregation:** The process of splitting the data, for example into train and test sets.

**Environment (runtime):** The environment where a software runs. In mlflow it is described by the conda.yml file (or the equivalent Dockerfile if using Docker).

**Experiment:** A tracked and controlled execution of one or more related software components, or an entire pipeline. In W&B the experiment is called group.

**Hyperparameters:** The parameters of a model that are set by the user and do not vary during the optimization or fit. They cannot be estimated from the data.

**Job Type:** Used by W&B to distinguish different components when organizing the ML pipeline. It is mostly used for the visualization of the pipeline.

**Machine Learning Pipeline:** A sequence of one or more components linked together by artifacts, and controlled by hyperparameters and/or configurations. It should be tracked and reproducible.

**Project:** All the code, the experiments and the data that are needed to reach a particular goal, for example, a classification of cats vs dogs.

**Run:** The minimal unit of execution in W&B and in all tracking software. It usually represents the execution of one script or one notebook, but it can sometimes contain more; for example, one script that spawns other scripts.