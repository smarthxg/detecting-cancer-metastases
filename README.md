# Breast Cancer Detection using Gigapixel Pathology Images

In this project we aim to implement a Multi-scale Inceptionv3 approach inspired from the paper

**[Detecting Cancer Metastases on Gigapixel Pathology Images](https://arxiv.org/abs/1703.02442)**

We use the CAMELYON 16 Multi Giga Pixel slides data. A set of 22 slides were sampled. Each slide has a corresponding mask which annotates the tumor region. We can access around 9 magnification levels.

Tissue Image               |  Mask Image
:-------------------------:|:-------------------------:
![Picture1](https://user-images.githubusercontent.com/34389844/119777900-6f0ee480-bee4-11eb-8c57-51bdd2cddc69.png) | ![Picture3](https://user-images.githubusercontent.com/34389844/119778014-91a0fd80-bee4-11eb-831b-5bdc2c45d9cf.png)


## Methodology
- **Architectures used**: Inceptionv3 (Multi-scale) fine-tuned for layers > 150
- **Initial Weights**: Image Net
- **Sliding Window**: 80x80
- **Center**: 50x50
- **Loss used**: Binary Cross entropy loss
- **Magnifications**: (2, 3) and (3, 4) 
