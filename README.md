# CIRL: Controllable Imitative Reinforcement Learning for Vision-based Self-driving
This repo is a inofficial tensorflow  implemention  of  ECCV2018 Paper：[CIRL: Controllable Imitative Reinforcement Learning for Vision-based Self-driving](http://openaccess.thecvf.com/content_ECCV_2018/html/Xiaodan_Liang_CIRL_Controllable_Imitative_ECCV_2018_paper.html). The implementation is to run on [CARLA](https://carla.org/) 0.8.4 stable version only.

Different from the original implementation in CIRL paper, we build this codebase to provide a baseline for another paper, IPC: Instance-Aware Predictive Navigation inMulti-Agent Environments. So some components are different, including:
1. the termination condition of each episode is different.
2. the maximum speed is 20m/s instead of 10m/s in original CIRL paper.
3. the target is to drive as safely and fast as possible instead of reaching some preset destination.
4. the evaluation is based on a modified reward.

All difference is to align the implementation with IPC and [SPC](https://github.com/ucbdrive/spc) for fair comparison.

To pretrain the model, we provide a collected on CARLA 0.8.4 with full stack of information, such as action trajectories, depth map, RGB observations, segmentations and so on. Downlaod the dataset [here](https://drive.google.com/file/d/1gYXt1FMm3XGsit9RgT728_27BQ0J7Slq/view?usp=sharing).

To cite the CIRL paper with [bibtex](https://scholar.googleusercontent.com/scholar.bib?q=info:Ml2g5XIC5eEJ:scholar.google.com/&output=citation&scisdr=CgUKz4z3ENOmnA-CbW8:AAGBfm0AAAAAX_WHdW_guif7ggJAXkszTr-Yl14yx5Mu&scisig=AAGBfm0AAAAAX_WHdeDrBtkJddCPBRlgGfNFWEiz-k8s&scisf=4&ct=citation&cd=-1&hl=zh-CN).

If you use the codebase together with the agent definition borrowed from IPC or SPC, please cite them as well: [SPC](https://scholar.googleusercontent.com/scholar.bib?q=info:PynZpY5JqgkJ:scholar.google.com/&output=citation&scisdr=CgUKz4z3ENOmnA-NTvQ:AAGBfm0AAAAAX_WIVvQwrtFWZb4pc6YD-Qqy6yhdBhhV&scisig=AAGBfm0AAAAAX_WIVqR6BckfSXGPJEVYyBbwwG1WMFU_&scisf=4&ct=citation&cd=-1&hl=zh-CN) and [IPC]().
