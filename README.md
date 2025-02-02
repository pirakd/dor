# DeepOrienter
### Deep orienter of protein-protein interaction networks
This is the repository of the paper ["D'or: Deep orienter of protein-protein interaction networks"](https://doi.org/10.1093/bioinformatics/btae355)
<img src="scheme.jpg" width="600"/>

### Getting started
This project is 100% implemented in python. Authors used python 3.8 but it should run with similar versions as well.

Please see that you clone the repository together with the gene translator submodule by running:
```
git clone --recursive https://github.com/pirakd/DeepOrienter.git
```
To instaell required packages run:
``` 
pip install -r path/to/project/requirements.txt
```

### What's inside
- **Datasets used in the paper:** Can be found in [input](input) folder.  
- **Deep learning model**: found in [deep_learning/models.py](deep_learning/models.py)
- **Example of a parameter configuration**: in [presets.py](presets.py)
- **Train example script** in [scripts/main.py](scripts/main.py) and **model load and inference example script** in [scripts/inference.py](scripts/inference.py).
For this purpose we also added a pre computed [propagation scores file](input/propagation_scores/) generated using 5 AML patients and a [deep model](input/models/18_01_2023__17_57_15_354) trained using these propgation scores and KPI interactions. 
- **Implementations of two previous methods** mentioned in the paper: [D2D.py](D2D.py) and [Vinayagam.py](Vinayagam.py)


### License
DeepOrienter is MIT licensed, as found in the [LICENSE](LICENSE) file.
