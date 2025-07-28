# 安装Seurat v5：

#Enter commandsinR (or R studio,ifinstalled)
```R
install.packages('Seurat')
library(Seurat)
```
# 安装"BPCells","presto","glmGamPoi"
```R
setRepositories(ind =1:3, addURLs =c('https://satijalab.r-universe.dev', 'https://bnprks.r-universe.dev/'))
install.packages(c("BPCells","presto","glmGamPoi"))
```
# 安装 "remotes" "seurat-data" "azimuth" "seurat-wrappers"

```R
if (!requireNamespace("remotes", quietly = TRUE)) {
  install.packages("remotes")
}
install.packages('Signac')
remotes::install_github("satijalab/seurat-data", quiet = TRUE)
remotes::install_github("satijalab/azimuth", quiet = TRUE)
remotes::install_github("satijalab/seurat-wrappers", quiet = TRUE)
```

# 安装Seurat v4：

```R
remotes::install_version("SeuratObject","4.1.4", repos = c("https://satijalab.r-universe.dev", getOption("repos")))
remotes::install_version("Seurat","4.4.0", repos = c("https://satijalab.r-universe.dev", getOption("repos")))
```
# Older versions of Seurat：

#Install the remotes package install.packages('remotes')# Replace 'X.X.X' with your desired version
#链接：github.com/satijalab/seurat/releases
```R
remotes::install_version(package='Seurat',version= package_version('X.X.X'))
```
#Install the development version of Seurat：

```R
install.packages('remotes')
remotes::install_github(repo ='satijalab/seurat',ref='develop')
library(Seurat)
```

# Docker安装

```dockerpull satijalab/seurat:latest```

# 下载到本地进行安装
```R
install.packages(path_to_file, repos =NULL,type="source")
```
# 关注公众号，不迷路
![公众号二维码](https://raw.githubusercontent.com/NameAIAK/push-articles/master/pic/gongzhonghao.jpg)

# 加V进生信交流群
![个人二维码](https://raw.githubusercontent.com/NameAIAK/push-articles/master/pic/wechatcode.jpg)