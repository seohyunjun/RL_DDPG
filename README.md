# CONTINUOUS CONTROL WITH DEEP REINFORCEMENT LEARNING (a.k.a DDPG)

## paper
----
DDPG - [Continuous control with deep reinforcement learning(2015.9.9)](https://arxiv.org/abs/1509.02971)

<br>

## Code Environment
----
[OpenAI-gym](https://www.gymlibrary.dev/)
[Mujoco in M1](https://bnmy6581.tistory.com/146)
<br>

<br>

## Mac setting 
```shell
brew install cmake zlib
pip install 'gymnasium[all]'
pip install autorom # 0.42 버전 설치 (0.55 버전 mac m1 subprocess error)
AutoROM --accept-license (rom license Y 후 ale_py rom으로 파일 이동)
# mv /Users/[user_id]/[anaconda/conda/miniforge]/envs/[env_name]/lib/python3.8/site-pakage/AutoRom/rom /Users/[user_id]/[anaconda/conda/miniforge]/envs/[env_name]/lib/python3.8/site-pakage/ale_py/rom/

# require
brew install mpi4py # 
pip install tensorflow-macos # tensorflow-macos (v2 -> compat.v1 )
pip install torch
pip install gymnasium

# fix code 
# gymnasium return 2 parameter
# state, info = env.reset()
# env.step()
```

## Train
----
```bash
## DDPG train
python spinningup/spinup/algos/pytorch/ddpg/ddpg.py 

## test policy 
python -m spinup.run test_policy spinningup/data/ddpg/ddpg_s0 --norender

## DDPG test model plotting 
python -m spinup.run plot spinningup/data/ddpg/ddpg_s0 --norender

```

 
<br>

## Install Reference 

---- 

<br>

[pip install gym error](https://www.pygame.org/wiki/MacCompile)
<br>

[딥러닝 분산 학습 관련 연구, Deep learning travels(류성원)](https://lyusungwon.github.io/assets/publications/DistributedDeepLearningTrainingOverview.pdf)
<br>

[나만의 GYM 환경 만들기](https://www.youtube.com/watch?v=chVLag1NIAQ)
<br>

[Spinning UP](https://spinningup.openai.com/en/latest/user/installation.html)

<br>


## DDPG 

<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B31.jpeg" height=80% width=80% >
<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B32.jpeg" height=80% width=80% >
<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B33.jpeg" height=80% width=80% >
<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B34.jpeg" height=80% width=80% >
<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B35.jpeg" height=80% width=80% >
<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B36.jpeg" height=80% width=80% >
<img src="https://github.com/seohyunjun/RL_DDPG/blob/main/ppt/%E1%84%89%E1%85%B3%E1%86%AF%E1%84%85%E1%85%A1%E1%84%8B%E1%85%B5%E1%84%83%E1%85%B37.jpeg" height=80% width=80% >

