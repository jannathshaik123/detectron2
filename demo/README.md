
## Detectron2 Demo

We provide a command line tool to run a simple demo of builtin configs.
The usage is explained in [GETTING_STARTED.md](../GETTING_STARTED.md).

See our [blog post](https://ai.facebook.com/blog/-detectron2-a-pytorch-based-modular-object-detection-library-)
for a high-quality demo generated with this tool.

conda activate firasenv

cd demo

python demo.py --config-file ../configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml \
  --webcam\
  --opts MODEL.DEVICE cpu MODEL.WEIGHTS detectron2://COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x/137849600/model_final_f10217.pkl