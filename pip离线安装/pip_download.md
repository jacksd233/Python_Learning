# 使用pip离线安装python库

  首先使用pip download下载对应的库whl文件及配套环境库（以tensorflow为例，使用清华大学镜像源）

  `pip download tensorflow -i https://pypi.tuna.tsinghua.edu.cn/simple`
  得到所有tensorflow的相关whl文件，最好先创建文件夹存放

  `pip install --no-index --find-links . tensorflow --user`
  将文件夹上传到离线服务器，进入文件夹安装，加入`--user`是避免可能出现的提示环境错误。
