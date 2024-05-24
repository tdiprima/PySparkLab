"A NumPy version >=1.18.5 and <1.25.0 is required for this version of SciPy (detected version 1.26.1".

To resolve this warning, you should downgrade your NumPy version to be within the compatible range for your version of SciPy. You don't need to downgrade SciPy; instead, just adjust NumPy to a compatible version.

Here's how you can do it:

1. **Downgrade NumPy**: Install a compatible version of NumPy.

```bash
pip install numpy==1.24.3
```

This command installs NumPy version 1.24.3, which is within the required range for your SciPy version.

If you want to ensure compatibility for other packages, you can create a requirements file and use that for installing the dependencies:

1. Create a `requirements.txt` file with the following content:

```
numpy>=1.18.5,<1.25.0
scipy
```

2. Install the dependencies using `pip`:

```bash
pip install -r requirements.txt
```

This approach ensures that NumPy is within the required range, and SciPy (along with other dependencies) is installed correctly.

## Upgrade numpy

```sh
pip install --upgrade numpy
```

<br>
