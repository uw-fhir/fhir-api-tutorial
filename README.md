# Framingham Risk Calculator FHIR Tutorial 

## Prerequesites
**Install these on your system before the tutorials!**

- Anaconda: https://docs.anaconda.com/anaconda/install/
- A public github account: got to www.github.com and create an account if you don't already have one!
- 

### Test Your System


# First Steps
1. Clone the tutorial from Github.
    - [ ] Create an account on Github if you have not already.
    - [ ] Login to your [Github account](https://github.com/login)
    - [ ] Navigate to https://github.com/uw-fhir/fhir-calculator-tutorial.git

2. Clone your project to your computer 
    - [ ] Open a terminal or Git Bash
    - [ ] Navigate to a folder where you want to keep your project. For example:
            ```
            cd C:/Users/Piotr/code
            ```
    - [ ] Find the **project url** by clicking the `Clone or download` green button on your top right corner of your Github project page and copying it to your clipboard.
    - [ ] Run the following command in the terminal to clone this project into the chosen folder: 
        `git clone [url-copied-in-previous step]`
    - [ ] When you open your chosen folder, you should see the project files in a directory called `fhir-calculator-tutorial`.
3. Open your project folder in your text editor for this tutorial to be able to view and change the files. We'll be using VS Code - so if you're also using that editor, go to `File/Open Folder...` to accomplish this step. 


### Troubleshooting
If you are getting an error saying Anaconda can't find the `fhirclient` module, you have to make sure you're installing the package in a way that the jupyter environment can load it. If doing a global `pip install fhirclient` does not work:

1. Open your `Anaconda Prompt`. 
2. Type `jupyter console`.
3. Paste the following code to make sure fhirclient (or any other missing packages) are installed where Anaconda can access it.
```python
# Install a pip package in the current Jupyter kernel
import sys
!{sys.executable} -m pip install fhirclient
```
(see https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/ for more info)


