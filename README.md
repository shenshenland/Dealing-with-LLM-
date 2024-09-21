# Dealing-with-LLM-
Some Some pitfalls that may be encountered while deploying large models


Due to various LLM models, which are really different and their functions are different, then what we can do is always creating new environment and use different version of Python: 

A good example is Qwen 2.5 which need the module `transformers-stream-generator`, who require Python between 3.5 - 3.10, which means we have to use various Python Version. 

To deal with these, my ways are changing virtual environment. 

Now is How to create a virtual environment: 
如何新建一个虚拟环境：

## 第一步 ##
定位需要创建虚拟环境的地方 \
一般在G盘 \ 
`G:\cahche_place\Python version\Python10> （建环境的地方）  "G:\cahche_place\Python version\Python10\python.exe" -m venv qwen25 （使用python新建环境 qwen25）`

启动环境\ 
`.\qwen25\Scripts\activate`

进行跑程序：
`"G:\cahche_place\Python version\Python10\qwen25\Scripts\python.exe"`

关于如何通过Vscode使用确定新的kernel:

首先使用CTRL+shift+p命令： 打开命令交互面板， 在命令面板中可以输入命令进行搜索(中英文都可以)，然后执行。命名面板中可以执行各种命令，包括编辑器自带的功能和插件提供的功能 \
在打开的命令面板中输入下述命令，如下图所示： \
`Python: Select Interpreter`
找到虚拟环境的位置 \
安装基本的pip \ 
"g:/cahche_place/Python porject/Qwen25/Scripts/python.exe" -m ensurepip --default-pip \
g:/cahche_place/Python porject/Qwen25/Scripts/python.exe" -m pip install ipykernel -U --force-reinstall 
