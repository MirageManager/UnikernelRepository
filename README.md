# Unikernel Repository
This repository is used to maintain a list of available unikernels. The 
application server will download it at start-up. 
Only unikernels listed here can be used in MirageManager. The correct structure
of a unikernel repositroy is explained here:
```
https://gitlab.lrz.de/ga27pag/unikernel_skeleton
```
Or can be seen in the reference implementations.
Each entry must have the following structure: 
```JSON
{ 
  "name": "UnikernelName", 
  "git": "git_server.dom/user/project" 
}

```
The overall JSON in `main.json` is a list of such entries. If this repository
is not public, the machien running the applicaiton server should have access using 
ssh with a key-file.