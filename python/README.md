# Often encountered issues. 
## PYTHONPATH
When a python script cannot recognize the imported project package: should add the path to the parent project to $PYTHONPATH, write it in the !/.bashrc, and source it.
## Default python interpreter
The default python interpreter is the same one as the env used in the terminal in the vscode.

## argparse: a common command-line tool for additional arguments
[argparse](https://docs.python.org/3/library/argparse.html)

### pip show package version
```
pip show drake
```

### conda change python version
```
conda install python=3.9
```

### use placeholder in yaml file
In a yaml file we can define variables and placeholders for future use in the same file.
```
configuration:
  _target_: src.models.components.dual_RL_configuration.DualRLConfig
  dim_state: 2
  dim_control: 1

net_control:
  _target_: src.models.components.simple_dense_net.SimpleDenseNet
  input_size: "{dim_state}"
  lin_size: 64
  output_size: "{dim_control}"
```

