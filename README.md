# mgjeon.github.io

## Environment

```
git clone https://github.com/mgjeon/mgjeon.github.io
cd mgjeon.github.io
```

```
mamba create -n blog
mamba activate blog
mamba update -y mamba
mamba install -y python=3.10 ipykernel
pip install --upgrade pip

mamba install -y -c fastai nbdev
nbdev_install_quarto

mamba install -y pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
pip install --upgrade "jax[cuda11_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
pip install --upgrade tensorflow[and-cuda]==2.14

mamba install -y numpy scipy matplotlib sympy pandas plotly netcdf4 pyvista k3d ipywidgets
pip install --upgrade findiff numdifftools diffusers transformers ftfy accelerate
```

## Quickstart

Check blog in local
```
quarto preview
```

Remove metadata of ipynb files
```
nbdev_clean --fname posts/
```

Update main branch
```
git add .
git push
```

Publish the changes
```
quarto publish gh-pages
```