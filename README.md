# Slurm

## Introduction

### Terms

| Quality of Service (Qos) | conjunto de regras aplicado aos jobs. |

### What you need to know

| USERNAME | 

### What you can do

O sacctmgr é o comando do Slurm para consultar e gerir informação sobre utilizadores, contas e regras de utilização dos recursos.

```bash
sacctmgr show qos
```

O problema é que isto mostra demasiada informação. 


| maxjobspu | Maximum Jobs Per User | Maximum job que um utilizador pode por QoS |
|-|-|-|


sacctmgr show qos gpu_batch format=name,maxtresperuser,maxtres,maxjobspu,maxsubmitjobspu,grptres
      Name     MaxTRESPU       MaxTRES MaxJobsPU MaxSubmitPU       GrpTRES 
---------- ------------- ------------- --------- ----------- ------------- 
 gpu_batch    gres/gpu=2    gres/gpu=2                    10               


## Running

Verifying if the job is running

squeue -u USERNAME


JOBID PARTITION     NAME     USER ST       TIME  NODES NODELIST(REASON)















