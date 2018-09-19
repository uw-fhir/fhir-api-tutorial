# Framingham Risk Calculator FHIR Tutorial 

## Prerequesites
**Install these on your system before the tutorials!**

- Anaconda: https://docs.anaconda.com/anaconda/install/
- A public github account: got to www.github.com and create an account if you don't already have one!
- 

### Test Your System

### Troubleshooting
If you are getting an error saying Anaconda can't find the `fhirclient` module, you have to make sure you're installing the package in a way that the jupyter environment can load it. If doing a global `pip install fhirclient` does not work:

1. Open your `Anaconda Prompt`. 
2. Type `jupyter console`.
3. Paste the following code to make sure fhirclient (or any other missing packages) are installed where Anaconda can access it.
```python
# Install a pip package in the current Jupyter kernel
import sys
!{sys.executable} -m pip install
```
(see https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/ for more info)
