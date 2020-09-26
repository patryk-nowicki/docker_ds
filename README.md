# Data Science Stack repo 

Env is based on docker image: jupyter/datascience-notebook 

Container contains main _jupyter_-ized DataScience stack, like: 
  * R
  * Python 3 
  * Julia 1.5.0

DokcerHub [link](https://hub.docker.com/r/jupyter/datascience-notebook)
Image docks [link](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
GitHub Site [link](https://github.com/jupyter/docker-stacks)

Command to run container with mapped ports and volumes (_docekr_ds_ - is cloned GitHub repo - should be alligned)

`docker run -d -p 8888:8888 -v ~/Desktop/docker_ds:/home/jovyan/work jupyter/datascience-notebook`

All datasets are ignored in the repository, but  mainly _gdown_-ed from GoogleDrive, like:

```python
import gdown
url = 'https://drive.google.com/u/0/uc?export=download&confirm=1d1e&id=1IXzOffSk-jJHMYhBJdfrHRegKw1ycdr9'
output = 'data.csv'
gdown.download(url, output, quiet=False) 
```
