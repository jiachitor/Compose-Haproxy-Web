# Docker Compose Demo

## Docker Compose 简介
- `Dockerfile` 可以让用户管理一个单独的应用容器；
- `Compose` 则允许用户在一个模板（`YAML` 格式）中定义一组相关联的应用容器（被称为一个 project，即项目）
   - 例如一个 Web 服务容器再加上后端的数据库服务容器等

## 术语
- `服务`（`service`）：一个应用容器，实际上可以运行多个相同镜像的实例。
- `项目`(`project`)：由一组关联的应用容器组成的一个完整业务单元

> **Notes**
> - 一个`项目`可以由多个`服务`（`容器`）关联而成，`Compose` 面向项目进行管理


## 该项目结构
```bash
compose-haproxy-web
├── docker-compose.yml
├── haproxy
│   └── haproxy.cfg
└── web
    ├── Dockerfile
    ├── index.html
    └── index.py
```




