# Meta-Learning Shared Hierarchies

Code for [Meta-Learning Shared Hierarchies](https://s3-us-west-2.amazonaws.com/openai-assets/MLSH/mlsh_paper.pdf).

##### Running Experiments
```
python main.py --task AntBandits-v1 --num_subs 2 --macro_duration 1000 --num_rollouts 2000 --warmup_time 20 --train_time 30 --replay False AntAgent
```
The MLSH script works on any Gym environment that implements the randomizeCorrect() function. See the envs/ folder for examples of such environments.
# New Comments
* Make sure to add the root directiory to the PYTHONPATH by running: `export PYTHONPATH=$PYTHONPATH:<path to mlsh>`.
* For now, I manually added the new gym environments to the gym folder in my system. I will make that cleaner later.
