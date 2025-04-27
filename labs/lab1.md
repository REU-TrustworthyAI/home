[<img width=900 src="../img/logo_rit.png?raw=yes">](../README.md)   
[Home](../README.md) |
[Schedule](../schedule.md) |

## Research Computing Exercise

### 1. Login.
- open a terminal on your local machine
```
ssh RIT-USERNAME@sporcsubmit.rc.rit.edu
```
- Enter your password for your RIT account.
- Use DUO app to allow the access when nothing prompts:
![Screenshot 2025-04-27 161457](https://github.com/user-attachments/assets/781923b0-6b02-47e9-a58b-247ce56938f4)
- Once you have successfully logged in, check your account information:
```
[RIT-USERNAME@sporcsubmit ~]$  my-accounts
```
- Clone your GitHub repo:
```
[RIT-USERNAME@sporcsubmit ~]$ git clone https://github.com/REU-TrustworthyAI/YOUR-REPO.git
```
### 2. Learn basics of Slurm and Spack.
- Slurm tutorial: https://research-computing.git-pages.rit.edu/docs/slurm_quick_start_tutorial.html
- Spack tutorial: https://research-computing.git-pages.rit.edu/docs/software_tutorial.html

### 3. Run the example code in the interactive mode.
```
[RIT-USERNAME@sporcsubmit YOUR-REPO]$ sinteractive

Account [hilse,reu,rc-onboard]: reu
Core count: 2
Run time [Max: 12:00:00]: 0-6:0:0

If the Job cannot begin within 120 seconds, it will be auto canceled

Submitting Job!

[RIT-USERNAME@clx-a-01 YOUR-REPO]$ cd lab1
[RIT-USERNAME@clx-a-01 lab1]$ spack env activate default-ml-x86_64-24071101
[RIT-USERNAME@clx-a-01 lab1]$ python3 main.py
[RIT-USERNAME@clx-a-01 lab1]$ exit
```
## Submit a job
- Edit the run.sh file
- Submit a job using the run.sh file:
```
[RIT-USERNAME@clx-a-01 lab1]$ sbatch run.sh
```
- Show all your jobs:
```
[RIT-USERNAME@clx-a-01 lab1]$ squeue --me
```
- Cancel a job:
```
[RIT-USERNAME@clx-a-01 lab1]$ scancel JOB-NUMBER
```
- Cancel all your jobs:
```
[RIT-USERNAME@clx-a-01 lab1]$ scancel --me
```
- Log out:
```
[RIT-USERNAME@clx-a-01 lab1]$ exit
```
 
