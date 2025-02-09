一种新颖的针对自注意力头激活的量化策略，该策略考虑到自注意力头中激活的异质分布特征，能够有效捕获量化参数以最小化多头自注意力层中的近似误差，同时通过运行时估计来降低量化参数存储成本，在保证模型性能的前提下将模型量化为8比特。在此基础上，结合针对输入维度的模型剪枝算法，本文还进一步提出了一种视觉Transformer的量化剪枝联合优化算法，通过评估线性层输入序列各维度的重要性来实现有效剪枝。为了减少剪枝对模型准确度的影响，使用L1正则稀疏化重要性评分，实现更高的剪枝比例，极大提升了网络的轻量化和计算效率。在ImageNet-100数据集上的实验表明，本文所提方法不仅能够灵活节约内存，而且能达到与基准模型相当甚至更好的性能。
