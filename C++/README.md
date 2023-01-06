# Template
call a function with a keyword 'template' before the function name:
```
*builder-> template AddSystem<double>(system)
```
an explanation can be found in the [answer](https://stackoverflow.com/questions/610245/where-and-why-do-i-have-to-put-the-template-and-typename-keywords).

# Class and object-oriented programming
default constructor: [answer](https://en.cppreference.com/w/cpp/language/default_constructor)
protected constructor: [answer](https://stackoverflow.com/questions/1057221/what-are-practical-uses-of-a-protected-constructor#:~:text=A%20protected%20constructor%20can%20be,would%20have%20to%20declare%20these.)


## google test
install gtest from github and use it in cmake projects:
[link](https://gist.github.com/dlime/313f74fd23e4267c4a915086b84c7d3d)

## Eigen 
The version information of eigen is written in Eigen/src/Core/util/Macro.h; which include world version, major version, and minor version.

Eigen is a header-only library, which normally does not require installation, but one can still install it via cmake:\\
Download the eigen version from github;\\
```
cd /path/to/eigen/
mkdir build && cd build
cmake ..
sudo make install 
```

