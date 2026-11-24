# CAHRNet
## Environment
- [PyTorch >= 1.8](https://pytorch.org/)
- [BasicSR >= 1.3.3](https://github.com/xinntao/BasicSR-examples/blob/master/README.md)
- **Training with the example option:**

```
CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 python -m torch.distributed.launch --nproc_per_node=8 --master_port=4321 train.py -opt options/trian_CAHRNet.yml --launcher pytorch
```
**Tesing with the example option:**

```
python test.py -opt options/test_CAHRNet.yml
```
