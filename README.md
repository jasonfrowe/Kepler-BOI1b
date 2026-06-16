Make a venv

```bash
python -m venv .boi1
source .boi1/bin/activate
```

Install bls cuda submodule for Transitfit5 and BLS CUDA implementations.

```bash
git submodule update --init --recursive
```

install the package:

```bash
cd bls_cuda
pip install h5py
pip install -e .
```

install the Jupyter Kernel:

```bash
pip install ipykernel
python -m ipykernel install --user --name=boi1 --display-name="Python (boi1)"
```

to get limb-darkening coefficients, install the following:

```bash
pip install exotic_ld
```



