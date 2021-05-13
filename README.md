# Setting up your development environment

## Using python virtualenv

[Click here](Development Environment.txt)

## Using Miniconda

1. Download Miniconda3 from [here](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh)
2. Run `sh Miniconda3-latest-Linux-x86_64.sh` to install

### For Oh My Zsh

Add the below code to the `.zshrc` file to work with conda where `/home/devlop/apps` is a custom location where Miniconda3 is installed

```
# >>> conda initialize >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$('/home/devlop/apps/miniconda3/bin/conda' 'shell.bash' 'hook' 2> /dev/null)"
if [ $? -eq 0 ]; then
    eval "$__conda_setup"
else
    if [ -f "/home/devlop/apps/miniconda3/etc/profile.d/conda.sh" ]; then
        . "/home/devlop/apps/miniconda3/etc/profile.d/conda.sh"
    else
        export PATH="/home/devlop/apps/miniconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda initialize <<<

```

3. Now exit all terminal windows and run it again
4. Disable conda's base environment on startup using `conda config --set auto_activate_base false`
   Exit the terminal and run it again. Now you will see conda's base environment is disable on startup
5. Create a conda environment
   `conda create -n kaggle python=3.8.5`
   A conda environment is created with name `kaggle` which can be activated using:
   `conda activate kaggle`
