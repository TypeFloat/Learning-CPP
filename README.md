Learning-CPP

如果你想使用docker来运行，可以在项目的根目录下在终端输入下面的命令：

```bash
docker run --name cpp -it -v "$PWD":/app gcc:12
```

如果你的本地没有gcc的镜像，docker将会自动从docker hub上下载gcc的镜像。等待一会容器即可运行成功，因为使用了`-it`指令，因此容器运行后会进入交互模式，此时你可以在容器中进行编译运行，输入`cd /app`即可看到本项目的所有代码。