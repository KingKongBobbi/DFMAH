# DFMAH

**If the paper is accepted, the complete code will be uploaded soon.** :boom:
:calendar: : The complete code will be published within :one: month after the article is accepted.

## Training

### Processing dataset
Refer to [DFMAH](https://github.com/KingKongBobbi/DFMAH)

### Download CLIP pretrained model
Pretrained model will be found in the 30 lines of [CLIP/clip/clip.py](https://github.com/openai/CLIP/blob/main/clip/clip.py). This code is based on the "ViT-B/32".

You should copy ViT-B-32.pt to this dir.

### Start

After the dataset has been prepared, we could run the follow command to train.
> python main.py --is-train --dataset coco --caption-file caption.mat --index-file index.mat --label-file label.mat --lr 0.001 --output-dim 64 --save-dir ./result/coco/64 --clip-path ./ViT-B-32.pt --batch-size 128
