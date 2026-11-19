# 4DGS Viewer

在线地址：**https://leilei0330.github.io/4dgs_viewer_app_sll/**

基于 [SuperSplat Viewer](https://github.com/playcanvas/supersplat-viewer) 修改的 4D 高斯查看器，支持：

- **FreeTimeGS++**：`.ftgs` 单文件、`.ftgsx` 多段拼接播放清单；
- **TGH2**（4D-Gaussian-Splatting 系）：带时间属性（`t_t_0` / `t_scale_0` / `r_vel_*`）的 `.ply`；
- 普通静态 3DGS：`.ply`、`.sog`、`.compressed.ply` 等。

## 使用方法

打开在线地址后，**把模型文件直接拖进页面**即可播放：

- 单个 `.ftgs` 或 `.ply`：直接拖入；
- `.ftgsx` 播放清单：连同它引用的段文件一起拖入（拖整个文件夹也可以）；
- TGH2 场景包：`.ply` 连同 `scene.json` 一起拖入（没有 `scene.json` 也能播）。

文件只在你本机内存中解析，不会上传到任何服务器。

动画播放需要浏览器支持 **WebGPU**（新版 Chrome / Edge / Safari；不支持时静态内容仍可查看）。

本仓库只存放构建产物（由源码仓库的 `scripts/deploy-pages.sh` 自动发布），源码为私有仓库。
