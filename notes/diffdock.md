#cgas 


## Process
```mermaid
graph TD;

A[protein] 
B[small-molecule library] 
C[docked small-molecule library]
D[equibind]

A --> D 
B --> D 
D --> C


class A,B,C,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z internal-link;
```


## notes
* Used for [[blind docking]] 
* part of [[diffusion models]]

##  claim
[[@corsoDiffDockDiffusionSteps2022]]

## hypothesis  
[[diffusion models engable sota fragment docking]]



## links
https://www.loom.com/share/4627d08ae27e4ca0b80a1f4ed0d2a7ad
[Papers with Code - PDBBind Benchmark (Blind Docking)](https://paperswithcode.com/sota/blind-docking-on-pdbbind?p=diffdock-diffusion-steps-twists-and-turns-for)
[](https://github.com/labdao-apps/diffdock)[https://github.com/labdao-apps/diffdock](https://github.com/labdao-apps/diffdock)
[Diffdock - a Hugging Face Space by simonduerr](https://huggingface.co/spaces/simonduerr/diffdock)