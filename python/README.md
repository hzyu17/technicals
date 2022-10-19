# Often encountered issues. 
## PYTHONPATH
When a python script cannot recognize the imported project package: should add the path to the parent project to $PYTHONPATH, write it in the !/.bashrc, and source it.

# Import module from parent directory
When building a package, it is quite often to import module from parent directories. \
One way of doing this is using \
```
dir = path.path(__file__).abspath()
sys.path.append(dir.parent.parent)
```


