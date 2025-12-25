几个重要的指令

安装包
python -m pip install -e ./exts/bipedal_locomotion

python -m pip install -e ./rsl_rl

训练
python3 scripts/rsl_rl/train.py --task=Isaac-Limx-PF-Blind-Flat-v0 --headless

运行
python3 scripts/rsl_rl/play.py --task=Isaac-Limx-PF-Blind-Flat-Play-v0 --checkpoint_path=path/to/checkpoint

训练修改机器人数量
python3 scripts/rsl_rl/train.py --task=Isaac-Limx-PF-Blind-Flat-v0 --headless --num_envs=100


运行指定模型
python3 scripts/rsl_rl/play.py --task=Isaac-Limx-PF-Blind-Flat-Play-v0 --checkpoint_path=./logs/rsl_rl/pf_tron_1a_flat/2025-12-25_15-40-11/model_1.pt

从指定模型开始训练修改机器人数量
python3 scripts/rsl_rl/train.py --task=Isaac-Limx-PF-Blind-Flat-v0 --headless --num_envs=4096 --checkpoint_path=./logs/rsl_rl/pf_tron_1a_flat/2025-12-25_15-40-11/model_1.pt