# BYOL model for Classification

I am using the BYOL over SimCLR as BYOL (Bootstrap Your Own Latent) offers several advantages over SimCLR (Simple Framework for Contrastive Learning of Visual Representations):

### **No Negative Pairs**
- **SimCLR**: Relies on the concept of contrastive learning with negative pairs. It requires large batch sizes to ensure a diverse set of negative examples, which helps in pulling together representations of similar images while pushing apart representations of dissimilar images.
- **BYOL**: Does not use negative pairs. Instead, it focuses on learning by predicting the representations of different augmented views of the same image.
- **Advantage**: By eliminating the need for negative pairs, BYOL simplifies the learning process and reduces the dependency on large batch sizes, making it more efficient and accessible, especially for users with limited computational resources.


___

# Resources

Paper link - https://arxiv.org/abs/2006.07733

Thanks to <a href=https://github.com/lucidrains>Phil Wang</a> for providng the torch implementation of BYOL

Torch implementation of BYOL - https://github.com/lucidrains/byol-pytorch

Also thanks to <a href=https://www.youtube.com/@YannicKilcher>Yannic Kilcher</a>, for the excellent explanation of the BYOL paper

Youtube Explanation - https://www.youtube.com/watch?v=YPfUiOMYOEE


