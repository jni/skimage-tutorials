# Preparation

## Format

The tutorial consists of lecture segments, followed by hands-on
exercises.  We strongly encourage you to bring a laptop with all the
required packages installed in order to participate fully.

## Software required

- Python

  If you are new to Python, please install the
  [Anaconda distribution](https://www.anaconda.com/distribution/) for
  **Python version 3** (available on OSX, Linux, and Windows).
  You will also need to install [napari](https://napari.org), using
  either `pip install napari` or `conda install -c conda-forge napari`.
  Make sure you execute those commands in the appropriate environment. If you
  are not sure what that means, it might be a good idea to come early to the
  session to ask the organisers for help.

  If you are comfortable with environments, feel free to use your favorite
  distribution, but please ensure the requirements below are met:

  - scikit-image >= 0.17
  - numpy >= 1.12
  - scipy >= 1.0
  - matplotlib >= 2.1
  - notebook >= 4.0
  - scikit-learn >= 0.18
  - pandas >= 0.25
  - napari >= 0.3

  For conda users, we have provided a conda environment that should work well
  for the workshop. Once you have downloaded the lecture materials (see
  "Download lecture materials", below), you can find the environment definition
  in the file `environment.yml`. Once you are at the root of the repository,
  you can create the environment with:

  ```bash
  conda env create -f environment.yml
  conda activate skimage-tutorial
  ```

  Please see "Test your setup" below.

- Jupyter

  The lecture material includes Jupyter notebooks.  Please follow the
  [Jupyter installation instructions](http://jupyter.readthedocs.io/en/latest/install.html),
  and ensure you have version 4 or later and notebook version 6 or later:

  ```bash
  $ jupyter --version
  jupyter core     : 4.6.3
  jupyter-notebook : 6.0.3
  ...
  ```

  The traditional Jupyter notebook interface is more stable than Jupyter Lab and is recommended for this workshop.

## Download lecture materials


### Option 1: using git

If you are familiar with git, you can clone the repository at
https://github.com/jni/skimage-tutorials.

```
git clone --depth 1 https://github.com/jni/skimage-tutorials
```

We may make editorial corrections to the material until the day before
the workshop, so please execute `git pull` to update before class.

### Option 2: download a zip file

Download the file at:

https://github.com/jni/skimage-tutorials/archive/monash-df-2020-08.zip

Unzip it, then start a jupyter notebook inside the archive.

## Test your setup

Please switch into the repository you downloaded in the previous step,
and run `python check_setup.py` to validate your installation.

On my computer, I see (but your version numbers may differ):

```
[✓] scikit-image  0.18.dev0
[✓] numpy         1.18.4
[✓] scipy         1.4.1
[✓] matplotlib    3.2.1
[✓] notebook      6.0.3
[✓] scikit-learn  0.23.0rc1
[✓] pandas        1.0.3
[✓] napari        0.3.6
```

**If you do not have a working setup, please contact the instructors.**

## After the workshop

The lecturers will upload our completed notebooks to the
`monash-df-2020-08-completed` branch. You can download it with git by first
saving your copy and then fetching that branch:

```
git commit -a -m "Work completed in class"
git fetch origin monash-df-2020-08-completed
git switch monash-df-2020-08-completed
```

**Or** you can download them directly at:

https://github.com/jni/skimage-tutorials/archive/monash-df-2020-08-completed.zip


