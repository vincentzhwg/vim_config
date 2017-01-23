# vim_config

`vim`配置文件，特别适用于`golang`工程师使用。

## 主要特性有：
* 集成`vim-go`插件
* 集成`YouCompleteMe`插件
* 集成`tagbar`插件
* 集成`ctrlp`插件


### 为了兼容`YouCompleteMe`，可能需要升级`vim`

`YouCompleteMe`对于`vim`版本有一定要求，如果发觉不满足，需要进行升级。下面给出在`ubuntu`环境下通过`apt`进行升级的解决方案。

    sudo apt-get install python-software-properties
    sudo apt-get install software-properties-common

先通过以上两行命令，使`ubuntu`安装上`add-apt-repository`命令，然后再通过以下命令升级`vim`。

    sudo add-apt-repository ppa:fcwu-tw/ppa  
    sudo apt-get update
    sudo apt-get install vim

至于其他发行版本的系统，请自行寻找方法进行`vim`的升级，以满足`YouCompleteMe`的要求。或者屏蔽卸载掉`YouCompleteMe`插件，但这样就损失了非常重要的自动补全的功能了，不太值得。或者替换成别的自动补全的插件，不过效果可能远远不如该插件，所以最好还是升级`vim`以满足该插件要求，这样的升级努力的付出，还是非常值得的。

## 安装方法

为了保持各种插件的`git`状态，所以采用了压缩包的方式，请先从以下链接将压缩包`vim_config.tar.gz`下载到本地

    [http://pan.baidu.com/s/1eSDSjOA]http://pan.baidu.com/s/1eSDSjOA

先清干净本地的vim环境，以备后面的安装

    rm ~/.vim{,rc} -rf

然后解压缩下载回来的文件到对应的位置即可

    tar zxvf vim_config.tar.gz -C ~/

