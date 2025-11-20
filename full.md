# C-S-H 体系机器学习势

# 介绍

本工作开发了一个神经进化机器学习势（NEP），适用于 tobermorite 和 C-S-H体系，通过预测tobermorite的结构和机械性能来证明 NEP的多功能性，并首次应用于非晶构型的MD模拟。该存储库提供了NEP模型的数据集、训练脚本、MD 示例以及各类计算脚本。

# 目录结构

![](images/a48ad8c36d6e05bfac7ed8f6bbaffe62dae296dcbfe896850e652a51a38d5cb2.jpg)

# 使用方法

# 1、 NEP训练/测试

运行以下命令：

cd 01-NEP-tob-C-S-H ln -s train-440.xyz train.xyz ../../ GPUMD-master/src/nep &

# 2、 MD 模拟

本 示 例 基 于 GPUMD 运 行 。 GPUMD 源 代 码 和 编 译 请 参 考 官 方 安 装 指南 https://gpumd.org/installation.htmlcd 02-Examples-MD/Tobermorite-NPTln -s model-9A.xyz model.xyz../../ GPUMD-master/src/gpumd>nep.log &说明：本 NEP 势函数 也可以在 LAMMPS 中使用。只需在 LAMMPS 中编译并启用 NEP 相关模块。