# Project: Image Processing Package
## Course by: [Karina Kato](https://www.linkedin.com/in/karina-kato-4b2a56182/)
### Course: Create a Image Processing package in Python - by Digital Innovation One

### Description:
the package "image_processing_python_test" it's used for:

- module - Processing:
  - Correspondência de histograma;
  - Similaridade estrutural;
  - Redimensionar imagem;

- module - Utils:
  - read the imagem;
  - save the imagem;
  - Plot the imagem;
  - show the graphic result;
  - Plot the histogram;
---------------------------------------------
## how to setup the package in the Pypi envirement:

- [x] instaled the leasted versions of  "setuptools" and "wheel"

```
py -m pip install --user --upgrade setuptools wheel twine
```

- [x] after instaled the packages check if the in the main project folder contain the following folders:
  - [x] build;
  - [x] dist;
  - [x] image_processing.egg-info.

- [x] Now you need just upload the folder to Pypi test environment, using the Twine :

```
py -m twine upload --repository testpypi dist/*
```

- [x] After run the command above the promp will ask the user and password. after that the project will be hosted in Pypi.

### Note: the project made by Karina it's only used for testing propurses.
----------------------------------------------------
## Test in Local machine : after hosted in Pypi:

- [x] Install dependecies
```
pip install -r requirements.txt
```

- [x] Install the packages 

use the package manager to install the package ```pip install -i https://test.pypi.org/simple/ image-processing ```

```bash
pip install image-processing-test
```
-------------------------------------------------
## how to import the package in other projects 

```python
from image-processing.processing import combination
combination.find_difference(image1, image2)
```

## Licença
[MIT](https://choosealicense.com/licenses/mit/)
