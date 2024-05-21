# Code and datasets for SEraser

The code we utilized and the corresponding data have been submitted anonymously. To execute, please proceed as per the following steps:


## Setup

In a conda env with pytorch / cuda available, run:
```
pip install -r requirements.txt
```


## Download

For convenience, we pack the subsets of datasets and they are available './data/(e.g., CamelDeer)'. Please change the `ROOT_DIR` in `fine_tune_blip.py`. The pretrained VLFMs is available on Lavis (a widely-used repository).

## Inference

The provided `fine_tune_blip.py` can be run on single-gpu automatically and you need `A100 GPU` for inference:
```
python3 fine_tune_blip.py \
--root_dir /path/of/datasets \
--dataset_name dataset_model (e.g., 'Waterbirds_clipB32')
```

Note that you should make sure that all checkpoints and its config are compiled following **Lavis**.
