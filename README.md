# 使用 docker-compose 一键启动

```shell

请先安装 docker-compose 程序！！！

例如在 debian 11 系统中:

apt update && apt install docker-compose

```

<br>

# docker-mcsm_发布版

## Usage

```shell

git clone https://github.com/zijiren233/docker-mcsm

cd ./docker-mcsm/releases

docker-compose up -d --build

```

- 发布版 web(前端): http://ip:23333

- 发布版 daemon(后端): http://ip:24444

- 发布版中不携带 java,要运行 java 程序请在 mcsm面板->环境镜像->环境镜像管理->新建镜像中自行构建

    - 实例设置中的进程启动方式选择 `虚拟化容器`

- 关闭服务器请进入到 docker-compose.yml 文件目录运行 `docker-compose stop`

    - 运行 `docker-compose down` 来移除容器

<br>

# docker-mcsm_开发版

## Usage

```shell

git clone https://github.com/zijiren233/docker-mcsm

cd ./docker-mcsm/dev

docker-compose up -d --build

```

- 开发版 UI(网页前端): http://ip:8080

- 开发版 MCSManager(控制面板端): http://ip:23333

- 开发版 Daemon(守护进程): http://ip:24444