单物体 
外型和颜色 
解耦=>可编辑 
自由视角过渡 

latent feature => 3d空间可视化 => 对latent feature的调整映射到最终渲染结果的变化。比如不同颜色对$\Delta z_a$的影响，旋转角度对$\Delta z_s$的影响，

可以参考nerf position encoding的一些可视化方法，最开始提出也很多人不理解pos encode的含义


* 3d空间特征空间的可视化
* 3d空间的交互探索

2个隐空间 

单独隐空间：shape https://arxiv.org/pdf/2110.02624.pdf

神经元 对应 渲染部分 https://arxiv.org/pdf/1911.06971.pdf

一个小想法，如果学习这篇的方法，将变化量的representation使用某个模型的generator映射到一个volume data中，然后用某种transfer function用体渲染的方式得到结果。但现在问题是，generator内部其实是隐式场，并不是显式地将3d空间中各个位置的color和density真的算出来了，

某种意义上，如果抛弃掉clip的影响，其实也只是换了一种方式去编辑nerf罢了。所以我认为我们需要先明确，我们想做的到底是从clip embedding的隐空间中提取3d空间的信息；还是从nerf中提取分离的shape和appearance信息

~~《Instruct-NeRF2NeRF: Editing 3D Scenes with Instructions》~~