# Taichi Newsletter for March

ISSUE 11 - April 10, 2023

Another month of exploring the fascinating world of Taichi. With an array of exciting new features, Demos, and blogs, we invite you to join us for the latest update of Taichi!

## 📌Highlights

- [Taichi NeRF](https://github.com/taichi-dev/taichi-nerfs) is released. Train your own 3D world!

- [Taichi v1.5.0](https://github.com/taichi-dev/taichi/releases/tag/v1.5.0): Taichi Runtime (TiRT) now supports Apple's Metal API and OpenGL ES for compatibility on old mobile platforms. 

##  ⚙️ Releases & Development

**Taichi v1.5.0 is available! See what's new:**

- Taichi Runtime (TiRT) now supports Apple's Metal API and OpenGL ES for compatibility on old mobile platforms.
- Taichi AOT fully supports float16 dtype.
- Out-of-bound checks are now supported on ndarrays.
- Python Frontend: LLVM-based backends (CPU and CUDA) now support returning structs, including nested structs containing vectors and matrices.
- The atomic operations for half2 data type (used for half-precision floating-point numbers) have been optimized in CUDA backend.
- Metal, OpenGL, AMDGPU, DirectX 11, CPU, and CUDA are supported on GGUI backend.

Hurry up and experience the new features 👉 `pip install -U taichi==1.5.0`.

193 PRs have been merged and 37 issues resolved this month.👏

## 🌟 Featured Repos & Projects

This is a [2D Eulerian fluid solver implemented](http://github.com/Lee-abcde/2DEulerianFluidSolver/tree/main) using the Taichi programming language, which achieves advanced functionality with a implementation of only 300 lines of code. Specifically, this solver enables interactive manipulation of the water surface through mouse interactions, as well as enhanced fluid dynamics through the addition of vorticity calculations. Additionally, this solver supports the flexibility to switch the fluid’s background image, with the images located in the designated img directory.

![](https://user-images.githubusercontent.com/124654014/231320221-db5038ea-6e18-4f9e-98e3-801d0eae21e0.gif)

[This project](https://github.com/sillsill777/SPH-Fluid-Simulation) is based on SPH Taichi. In this project with the SPH formalism, [sillsill777](https://github.com/sillsill777) will numerically solve fluid equations which govern the movement of fluid flow. Furthermore, they will consider several effects governing fluid motion such as viscosity and surface tension. The author will also handle the issue of Fluid-Rigid coupling.

![](https://user-images.githubusercontent.com/124654014/231322232-21962c8e-40fa-4c20-ab83-0b0c37de75e6.gif)

High Viscosity case with viscosity set to 0.5

![](https://user-images.githubusercontent.com/124654014/231322239-e9494f74-0943-492a-8f25-63f12f9a60f3.gif)

Two fluid block setting

- **[使用 Taichi NeRF 进行三维重建](https://mp.weixin.qq.com/s/524hkvbkGzryKNyq9brhpg)**

NeRF 技术可以通过一系列 2D 图像对场景进行准确和详细的重建。这个 Demo 展示了 Taichi NeRF 根据不同角度捕捉办公室的多个图像，并生成高质量的 3D 模型，生成的模型可以从任何视角进行探索和可视化。欢迎大家使用 [Taichi NeRF](http://github.com/taichi-dev/taichi-nerfs) 创造 3D 场景！

![](https://user-images.githubusercontent.com/124654014/231321710-8313da5a-b45c-49c9-a671-6ed051d1c71b.gif)

## 📝 精选博客

**📚 [数值计算从入门到进阶，不能错过这些高质量好书](https://mp.weixin.qq.com/s/yXltvJp6YMhCN7uqXn9IMg)**

我们邀请了几位 Taichi 数值计算兴趣小组成员，请大家介绍一些「亲测好用」的学习资料，过程中收获了 10 多本书籍和论文推荐。包含基本原理和方法，以及如何应用相关方法解决工程和科学问题。

**🔢 [LBM 理论基础是如何推导出来的？Taichi 在数值计算方面有哪些优势?](http://zhuanlan.zhihu.com/p/613851844)**

作者 tau 先从大家比较熟悉的基于连续介质假设而建立的宏观流体力学基本方程入手进行描述，之后简单介绍了微观分子动力学的控制方程并引出介观气体动理论的基本方程——Boltzmann 方程，还写了一个双分布函数的小 Demo 来展示如何利用数值方法来对格子 Boltzmann 方程进行求解。

**💻 [从 Houdini 生成输出四面体网格，有哪些好用的方法?](zhuanlan.zhihu.com/p/613817030)**

在 FEM 和 PBD 等软体模拟中，常常需要四面体网格。尤其是可控的，可自由修改的，不同分辨率的网格。Houdini 中的 tetconform 节点能生成很好质量的节点，并且很好修改。但是，Houdini 是不能直接输出四面体的。因此作者北斗分享了最近探索的途径，从 Houdini 中利用 Python 节点输出 tetgen 格式的四面体。

## 🧑‍💻 贡献者力量

感谢社区同学们在 Taichi 项目中的贡献❤️

- **taichi-nerfs**

@erjanmx: Fix readme typo #23

@JiahaoPlus: [bug] Fix utils depth2img by importing cv2 and numpy #17

- **taichi**

@ritobanrc: [doc] Handle 2 digit minor versions correctly #7535

@NextoneX: [Doc] Update gui_system.md, remove unnecessary example #7487

@schuelermine: [docs] Reword words of warning about building from source #7488

## 🙋‍♂️ Taichi 小课堂

**🤷‍♂️ 如何使用 Taichi 的 math 模块进行复数算术运算？**

⭐️ 可以使用 2D 向量（ti.math.vec2）表示复数，vec2 中两个数字分别表示复数的实部和虚部，例如使用 ti.math.vec2(1, 1)来代表复数 1+1j。

## 扫描以下二维码关注我们～
![](https://user-images.githubusercontent.com/124654014/231324202-21baace2-3b4f-47ac-a9d0-018617f7df9d.jpeg)











