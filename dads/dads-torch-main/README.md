
# PyTorch implementation Dynamics-Aware Discovery of Skills (DADS).
The ``dads-torch`` repository contains all modules needed for the implementation of [DADS](https://arxiv.org/abs/1907.01657).
In addition, all routines for off-policy training and zero-shot execution in MujoCo environments are supported.
The RL algorithm SAC used here is a modification of the implementation from [pranz24](https://github.com/pranz24/pytorch-soft-actor-critic).


### Run experiments
Change the required test point directory in the ``off_policy.yaml`` file and run

    python -m dads.main.main mode=dads_train

then change the directory in the ``zero_shot.yaml`` file to the required directory containing the trained networks and
execute

    python -m dads.main.main mode=dads_eval
