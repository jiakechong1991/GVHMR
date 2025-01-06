


# 加载 动作识别的数据：
data=torch.load("./outputs/demo/dance1/hmr4d_results.pt")

'smpl_params_global'：# 其他相机视角
    body_pose torch.Size([1147(帧率), 63(21个关键点相对旋转)]) 
    betas torch.Size([1147, 10]) # 10个SMPL的shape参数
    global_orient torch.Size([1147, 3])  # root朝向
    transl torch.Size([1147, 3])  # root位移


'smpl_params_incam'  # 原生摄像机视角
    body_pose torch.Size([1147(帧率), 63(21个关键点相对旋转)]) 
    betas torch.Size([1147, 10]) # 10个SMPL的shape参数
    global_orient torch.Size([1147, 3])  # root朝向
    transl torch.Size([1147, 3])  # root位移


'K_fullimg'： [1147, 3, 3]
'net_outputs： # 各个层的网络输出结果