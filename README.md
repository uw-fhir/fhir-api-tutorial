# FHIR API Tutorial 

## Prerequisites
**Install these on your system before the tutorials!**

- Anaconda: https://docs.anaconda.com/anaconda/install/
- A public github account: got to www.github.com and create an account if you don't already have one!
- On Windows, Git bash is recommended: https://gitforwindows.org/

### Test Your System


# First Steps
1. Clone the tutorial from Github.
    - [ ] Create an account on Github if you have not already.
    - [ ] Login to your [Github account](https://github.com/login)
    - [ ] Navigate to https://github.com/uw-fhir/fhir-api-tutorial.git

2. Clone your project to your computer 
    - [ ] Open a terminal (Mac/Linux) or Git Bash (Windows)
    - [ ] Navigate to a folder where you want to keep your project. For example:
            ```
            cd C:/Users/Piotr/code
            ```
    - [ ] Find the **project url** by clicking the `Clone or download` green button on your top right corner of your Github project page and copying it to your clipboard.
    - [ ] Run the following command in the terminal to clone this project into the chosen folder: 
        `git clone [url-copied-in-previous step]`
        - alternatively, you can also download the repo as a zip file
    - [ ] When you open your chosen folder, you should see the project files in a directory called `fhir-api-tutorial`.
3. Make sure you can run jupyter and view the notebooks: `jupyter notebook .`


### Troubleshooting
PLEASE NOTE: As of September 2020, the version of the fhirclient module that is available from pip is DSTU3, not R4. R4 is the current and preferred API version. Install the package from the git source to get the R4 version: `pip install git+https://github.com/smart-on-fhir/client-py.git`


If you are getting an error saying Anaconda can't find the `fhirclient` module, you have to make sure you're installing the package in a way that the jupyter environment can load it. 

1. Open your `Anaconda Prompt`. 
2. Type `jupyter console`.
3. Paste the following code to make sure fhirclient (or any other missing packages) are installed where Anaconda can access it.
```python
# Install a pip package in the current Jupyter kernel
import sys
!{sys.executable} -m pip install git+https://github.com/smart-on-fhir/client-py.git
```
(see https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/ for more info)


