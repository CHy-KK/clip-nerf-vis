
1. 《GRAF: Generative Radiance Fields for 3D-Aware Image Synthesis》 2020
https://github.com/autonomousvision/graf
备注：《GIRAFFE: Representing Scenes as Compositional Generative Neural Feature Fields》2021 改进点之一是解决了graf的single scene和single object问题
2. 《Editing Conditional Radiance Fields》
https://github.com/stevliu/editnerf
3. 《Efficient Geometry-aware 3D Generative Adversarial Networks》
https://github.com/softwarearchitect817/Efficient-Geometry-aware-3D
4. 《CG-NeRF: Conditional Generative Neural Radiance Fields》
将clip embedding作为condition输入condition generator，但是不开源
5. ~~《Instruct-NeRF2NeRF: Editing 3D Scenes with Instructions》~~
https://github.com/ayaanzhaque/instruct-nerf2nerf/tree/main
~~用已有的nerf渲染结果配合clip输入得到新的nerf渲染，模型通过2d的diffusion model更新捕获视点的图像内容，随后通过标准Nerf的训练过程来辅助计算编辑内容~~
使用优化的方式而非隐空间方法，不适用于我们的工作
6. 
