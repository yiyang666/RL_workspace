# 主目录结构
RL_workspace/
# 学习资产
├── learning/
    ├── easy-rl/    # 强化学习教材 + 实验 playground
    ├── pytorch_basics/
    ├── gymnasium_playground/
    ├── mujoco_playground/
    ├── ppo_scratch/
    └── diffusion_policy_playground/
# 长周期维护项目
├── projects/
    ├── humanoid_rl/
    ├── quadruped_navigation/
    ├── rov_control/
    └── isaaclab_research/
# 实验结果
├── experiments/
    ├── exp_001_ppo_cartpole/
        ├──logs/
        ├──tensorboard/
        ├──videos/
        ├──configs/
        ├──metrics/
        └──notes.md
    ├── exp_002_sac_halfcheetah/
    └── exp_003_g1_walk/
# 数据
├── datasets/
    ├── d4rl/
    ├── robomimic/
    ├── isaac_assets/
    └── rosbags/
# 环境资产！重要！不放代码！不放实验！环境定义！
├── docker/
    ├── rl_base/     # 基础环境，用于派生
    ├── rl_learning/
        ├── Dockerfile
        ├── docker-compose.yml
        ├── requirements.txt
        ├── scripts/
        └── README.md
    ├── mujoco/
    ├── isaaclab/
    ├── ros2/
    └── diffusion/
# 通用脚本和工具
├── scripts/
├── tools/
# 模型
├── checkpoints/
# tensorboard 日志
├── logs/
└── README.md


# 目录作用：
- rl_lab
    - 基础RL docker环境
- RL_workspace
    - 学习环境
    - 小实验环境

# 科学、系统的学习 RL-强化学习

## 设备资源汇总：
- MAC mini
    - 使用环境：居家使用/带到公司使用
    - SSH 连接 OMEN-ly 服务器 RL容器
- iPad pro
    - 充当mac使用
    - 公式手写推导
    - 观看学习视频
- OMEN-ly-5060
    - 角色：工作电脑
    - 风险控制：避免工作环境被污染和崩溃
    - 提供可视化环境
        - 由于服务器没有可视化界面，需要配合服务器进行使用
        - 重播训练结果进行观察
- Server-5090-ethan
    - 系统层：
        - 公共服务器上的个人用户空间
        - 小实验
        - 调试
        - 本地推理
        - 小模型
    - Docker层：
        - 强化学习训练
        - RL rollout
        - lsaacLab
        - mujoco
        - 大实验

