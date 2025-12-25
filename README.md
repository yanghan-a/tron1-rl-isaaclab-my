几个重要的指令
python -m pip install -e exts/bipedal_locomotion

cd bipedal_locomotion_isaaclab/rsl_rl
python -m pip install -e .
训练
python3 scripts/rsl_rl/train.py --task=Isaac-Limx-PF-Blind-Flat-v0 --headless

运行
python3 scripts/rsl_rl/play.py --task=Isaac-Limx-PF-Blind-Flat-Play-v0 --checkpoint_path=path/to/checkpoint
