# HackDisaster
Original dataset - 290 segmented images of damaged buildings. 

Notebooks:

-HackDisaster.ipynb - Resnet18 - U-Net model with resnet18 encoder. Patched dataset with size 300x300 and stride 150.

-HackDisaster_Swin.ipynb - Swin-Transformer - UNet model with Swin-Transformer as the backbone. Trained large pre-trained Swin model. The 3 last layers were unfrozen for training. Pretrained Swin requires images with size 224x224, so I added reshaping from 300x300 to 224x224.

-HackDisaster_Swin_emb_large01.ipynb - Swin-Transformer - UNet model with Swin-Transformer as the backbone. UNet with full image embedding and patch positional embedding to the model bottleneck. Trained large pre-trained Swin model. The 3 last layers were unfrozen for training. Created a new dataset with patch size 224x224 and stride 112 and saved corresponding embeddings alongside image and mask 
