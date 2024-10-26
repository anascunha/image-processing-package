# Project: Image Processing Package
## Project Author: Karina Kato
### Challenge: Creating an Image Processing Package with Python - Data Engineering Bootcamp with Python
[(click here to see my profile on the platform)](https://dio.me/users/ana_sara_sc)
#### Technology: Python
#### Date: 10/25/2024
-----------------------------------------
### Description
The "image_processing-test" package is used for:

- Processing module:
  - Histogram matching;
  - Structural similarity;
  - Resize image;

- Utils module:
  - Read image;
  - Save image;
  - Plot image;
  - Graph result;
  - Plot histogram;
---------------------------------------------
## Step-by-step configuration for hosting a Python package in the Test Pypi test environment

- [x] Installing the latest versions of "setuptools" and "wheel"

```
py -m pip install --user --upgrade setuptools wheel
```
- [x] Make sure the directory in the terminal is the same as the "setup.py" file

```
C:\User\anas\image-processing-package> py setup.py sdist bdist_wheel
```

- [x] After completing the installation, check if the following folders have been added to the project:
- [x] build;
- [x] dist;
- [x] image_processing_test.egg-info.

- [x] Just upload the files, using Twine, to Test Pypi:

```
py -m twine upload --repository testpypi dist/*
```

- [x] After running the above command in the terminal, you will be asked to enter your username and password. Once this is done, the project will be hosted on Test Pypi. Host it on Pypi directly.

### The goal here is not to use Karina's project to post on my personal Pypi profile, since the project is hers. I don't have any projects that can be used as a package yet.

### However, keep in mind that Test Pypi, as its name suggests, is just a testing environment. In order for the project to be available as a package for public use, it is necessary to host it on the official Pypi website. ----------------------------------------------------
## Local installation, after hosting on Test Pypi

- [x] Installing dependencies
```
pip install -r requirements.txt
```

- [x] Installing the package

Use the package manager ```pip install -i https://test.pypi.org/simple/ image-processing-test ```to install image_processing-test

```bash
pip install image-processing-test (Test Pypi)
```

## Author (who hosted the project on Test Pypi)
Ana Cunha

## License
[MIT](https://choosealicense.com/licenses/mit/)
