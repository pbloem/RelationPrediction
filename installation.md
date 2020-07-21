Install anaconda

Create a clean venv 
```bash
conda create -n rgcn-reference python=3.6
source activate rgcn-reference
```

Install tensorflow 1.4 (only works in pip)
```bash
pip install tensorflow==1.4
```

Install other dependencies
```bash
pip install theano
```

Run FB15k
```
python code/train.py --settings settings/fb15k.exp --dataset data/FB15k
```

Run WN18k
```
python code/train.py --settings settings/wn18k.exp --dataset data/wn18k
```

# Notes
* With current settings WN18 uses around