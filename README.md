# OBI-dataloader

## Usage

### Set up environment 

Install Anaconda and Git as instructed in the [aisynphys installation documentation](https://aisynphys.readthedocs.io/en/latest/installation.html)

After installing Miniconda, initialize Conda:

```bash
conda init

1. Download aisynphys repository 
```bash 
git clone https://github.com/alleninstitute/aisynphys aisynphys-repo

cd aisynphys-repo
```


2. Create virtual environment

From the `aisynphys-repo` directory: 
```bash
conda env create --name aisynphys --file desktop-environment.yml

conda activate aisynphys
```

3. Install the Jupyter Kernel. 
```bash
pip install ipykernel

python -m ipykernel install --user --name=aisynphys --display-name "Python (aisynphys)"
```
4. Install aisynphys:
```bash
python -m pip install -e .

cd ..
```

5. If you are using VSCode, open the Jupyter Notebook. In the notebook, select the kernel: **Python (aisynphys)**