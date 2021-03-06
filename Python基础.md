# Python基础
## Python解释器  
Python是一门解释型语言，代码必须通过解释器执行。Python存在多种解释器，分别基于不同语言开发，每个解释器有不同的特点，以下为常见的Python解释器：
- CPython：基于C语言开发，Python官网提供的版本
- IPython：基于CPython的交互式解释器
- PyPy：采用JIT技术，对代码进行动态编译，可以显著提高执行速度
- JPython：在Java平台运行的Python解释器，可以直接把Python代码编译成Java字节码执行
- IronPython：运行在微软.NET平台上，可以直接把Python代码编译成Net字节码

## Python包管理器
软件包源中的软件包数量巨大，版本多样，所以需要借助于软件源管理工具，常见的包管理器有：
- pip 是最常用的包管理工具，通过 pip install <packagename> 命令格式来安装软件包，使用的是 pypi 软件包源  
- conda 多用作科学计算领域的包管理工具，功能丰富且强大，使用的软件包源是 Anaconda repository 和 Anaconda Cloud，conda 不仅支持 Python 软件包，还可以安装 C、C++ 、R 以及其他语言的二定制软件包。除了软件包管理外，还能提供相互隔离的软件环境。
- Pipenv 是 Kenneth Reitz 在2017年1月发布的Python依赖管理工具，现在由PyPA维护。Pipenv 会自动帮你管理虚拟环境和依赖文件，并且提供了一系列命令和选项来帮助你实现各种依赖和环境管理相关的操作  
- Poetry 和 Pipenv 类似，是一个 Python 虚拟环境和依赖管理工具，另外它还提供了包管理功能，比如打包和发布。你可以把它看做是 Pipenv 和 Flit 这些工具的超集。它可以让你用 Poetry 来同时管理 Python 库和 Python 程序  
很多包管理工具不仅提供了基本的包管理功能，还提供了虚拟环境构建，程序管理的等功能!  
  
## Python虚拟环境
Python 应用经常需要使用一些第三方包或者模块，有时需要依赖特定的包或者库的版本，所以不能有一个能适应所有 Python 应用的软件环境，很多时候不同的 Python 应用所依赖的版本是冲突的，满足了其中一个，另一个则无法运行。解决这一问题的方法是虚拟环境。虚拟环境是一个包含了特定 Python 解析器以及一些软件包的自包含目录，不同的应用程序可以使用不同的虚拟环境，从而解决了依赖冲突问题，而且虚拟环境中只需要安装应用相关的包或者模块，可以给部署提供便利。常见的虚拟环境管理包有：
- pipenv
- virtualenv
- virtualenvwrapper


