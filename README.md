# ACCM

This is our implementation for the paper:

*Shaoyun Shi, Min Zhang, Yiqun Liu, and Shaoping Ma. 2018. [Attention-based Adaptive Model to Unify Warm and Cold Starts Recommendation.]() 
In CIKM'18.*

**Please cite our WWW'18 paper if you use our codes. Thanks!**

Author: Shaoyun Shi (shisy13@outlook.com)



## Environments

See in [requirements.txt](https://github.com/THUIR/ACCM/requirements.txt)

```
tensorflow_gpu==1.4.0
pandas==0.23.1
numpy==1.14.5
tqdm==4.23.4
```



## Datasets

- **ml-100k**: The processed ml-100k dataset can be found in [./dataset](https://github.com/THUIR/ACCM/dataset). The origin dataset can be found [here](https://grouplens.org/datasets/movielens/). The code for processing the data can be found in [./src/ml-100k.py](https://github.com/THUIR/ACCM).



## Example to run the codes		

```python
# ACCM with Cold-Sampling
python CSACCM.py --warm_ratio 0.9

# ACCM without Cold-Sampling
python CSACCM.py --warm_ratio 1.0
```

> Note that other codes ending with `*Model.py` is inherited by `CSACCM.py`

Last Update Date: Aug 25, 2018