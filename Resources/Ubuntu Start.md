* Firefox cannot synchronize  
    * 原来是Firefox的附加组件管理器不见了，我们只需要重新安装上即可: https://blog.csdn.net/JohnYu024/article/details/79763300  
    * Add-on manager link: http://mozilla.com.cn/thread-343905-1-1.html



* Latex 安装：
    > 要加中文：`\usepackage[UTF8]{ctex}`即可：https://jdhao.github.io/2018/03/29/latex-chinese.zh/ 
    * Linux下， 安装vscode
    * sudo apt-get install texlive-full cjk-latex latex-cjk-chinese
    * 安装 Latex Workshop 插件 

    * Debug:
        * 有一篇的Bibtex的Library未找到，结果显示所有reference有错



* No Wifi Model  
    * `iwconfig`: see whether there is a model called wlan0. If not, it means that the network card driver is not installed.  
    * `sudo lshw -c network`: see the model and vendor oationf the network card. For example, `BCM43142 802.11 b/g/m, vendor: Broadcom Corportion`  
    * For Broadcast network card:`sudo apt-get install`, `sudo apt-get bcmwl-kernel-source`
