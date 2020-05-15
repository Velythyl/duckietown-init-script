# Docs (General Cleanup):
https://docs.duckietown.org/DT19/AIDO/out/cm_sw.html
dts unusable if you dont dts --set-version

# RL brushup:

- [ ] Look at this series of videos https://www.youtube.com/watch?v=2pWv7GOvuf0
- [ ] Read survey paper https://arxiv.org/abs/1708.05866
- [ ] Read recent RL paper https://arxiv.org/pdf/1811.12560.pdf

# RL Cleanup:
Startpoint: https://docs.duckietown.org/DT19/AIDO/out/embodied_rpl.html

- [x] Make a script to init the repo, so that the Jetson docker can do it too [https://github.com/Velythyl/challenge-aido_LF-baseline-RPL-duckietown/issues/1]
- [ ] Make a script to train [IN PROGRESS]
- [ ] Make a script to do a submission automatically [IN PROGRESS]
- [ ] Fix bug that occurs when doing 34.4 of https://docs.duckietown.org/DT19/AIDO/out/embodied_rpl.html : 
![Image of bug](/roslaunch_bug.png?raw=true )


NOTE: initially, I wanted to make the init, sumbit, etc script a Makefile, but I realized a full-fledged script might be better at parsing args and at chaining commands together

# Logs:
5/6/2020 started to install stuff, installed dts, got stalled by the bug in https://docs.duckietown.org/daffy/AIDO/out/cm_first.html  
5/7/2020 turns out that the bug is only for that link https://docs.duckietown.org/daffy/AIDO/out/cm_first.html . It works fine for the pytorch and RL baselines. Fiddled with those a bit to learn the stack. Contacted Liam and sent me a lot of helpful resources. Started working on the "more up to date" RL, https://docs.duckietown.org/DT19/AIDO/out/embodied_rpl.html from https://github.com/PhilippeMarcotte/challenge-aido_LF-baseline-RPL-duckietown . Forked it here: https://github.com/Velythyl/challenge-aido_LF-baseline-RPL-duckietown . Started work on the init script for it in branch `create-script`.  
5/8/2020 Deadline for OS class TPs is May 10th: worked on tp3 autograder  
5/9/2020 worked on tp3 autograder  
5/10/2020 weekend break (mother's day)  
5/11/2020 worked on tp3 autograder  
5/12/2020 finished tp3 autograder, tp5 autograder  
5/13/2020 back on duckietown baybee! Figured out the `unkown runtime: nvidia` bug. Latest docker version completely ignores docker-compose.yml `version` tag, and thus the `runtime` flag is unkown, because it thinks it's using 3.x, apparently.  
5/14/2020 First time seeing a result!!! I call it brakedancing: the car just spins in circles without moving 10/10. Jokes asides, it's great seeing something for the first time  
