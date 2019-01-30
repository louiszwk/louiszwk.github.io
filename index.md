## docker 安装 mysql


第一步，从docker中拉取MySQL镜像

$ sudo docker pull mysql



$ sudo docker images



第二步，创建并启动一个MySQL容器

$ sudo docker run --name mysql -e MYSQL_ROOT_PASSWORD=123456 -p 3306:3306 -d mysql



查看容器运行状态：

$ sudo docker ps



第三步，测试连接MySQL

这里我使用navicat远程连接，连接MySQL前需要防火墙开放端口或者关闭防火墙。

开放端口：

$ sudo firewall-cmd --add-port=3306/tcp

关闭防火墙：

$ sudo systemctl stop firewalld

You can use the [editor on GitHub](https://github.com/louiszwk/louiszwk.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/louiszwk/louiszwk.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
