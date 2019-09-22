# NK.Blog

## 实现方案
### wyam [官网](https://wyam.io/)
使用wyam 来生成静态页面

#### 命令行使用
**1.安装**
> dotnet tool install -g Wyam.Tool

**2.生成新项目**
> wyam new --recipe Blog

**3.生成静态站点**
> wyam --recipe Blog

### Nginx
使用 nginx 来host
