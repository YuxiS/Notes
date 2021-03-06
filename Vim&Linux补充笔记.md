# Vim 笔记[learn x in y minutes]

## 初级操作

1. **syn on/off** 语法高亮开启/关闭

2. **ctrl+z** 挂起，**fg** 返回

3. **:w filename**  写入文件				 

4. **v **进入vision，可以选择代码

5. **/%s/word **全文查找

   | 关键字                    | 说明                                     |
   | ------------------------- | ---------------------------------------- |
   | ctrl+w c/o                | 关闭/只保留当前分屏                      |
   | **/word**                 | 向下检索word关键字                       |
   | **?word**                 | 向上检索word关键字                       |
   | **n**                     | 继续上一次操作                           |
   | **Ctrl + ]**              | 提取跳转当前光标下的word到定义           |
   | **ctrl + o**              | 返回跳转前位置                           |
   | __:set tages += ./tags__  | 指定tags文件，tags文件就是一个数据库文件 |
   | __:set number/nonu__      | 设置/隐藏行号                            |
   | **split/vsplit/new/vnew** | 分屏/垂直分屏/分屏打开新文件             |
   | __cc__                    |                                          |
   | __yy__                    | 复制游标所在行                           |
   | **4yy**                   | 复制当前光标一下4行                      |
   | __y1G__                   | 复制所在行到第一行所有数据               |
   | __yG__                    | 复制光标所在行到最后一行的所有内容       |
   | **p**                     | 粘贴复制板中的内容，和yy常用             |
   | **u**                     | undo，撤销上一步操作                     |
   | __dd__                    | 删除游标所在行（其余操作类似于yy）       |
   | **J**                     | 将光标所在行与下一行结合成同一行         |
   | **shift+d**               | 删除一行后保留空行                       |
   | :vs/sv                    | 垂直水平分屏                             |

**~/.vimrc** vim设置文件

​		__*永久设置可以在~/.vimrc（Ubuntu下）*__



****

# **Linux** 补充

* **ls -ltr** 查看文件生成顺序

* __ctags__[^ctags]

  ***Ctags: 扫描指定的源文件，找出其中所包含的语法元素，并将找到的相关内容记录下来***

  | command                    | comment                                         |
  | -------------------------- | ----------------------------------------------- |
  | __ctags --list-languages__ | 查看ctags支持的语言                             |
  | __ctags --list-kinds__     | 查看ctags可以识别和记录的语法元素               |
  | __ctags -R *__             | 对当前目录下所有ctags指出的语言格式文件生成tags |
  | __ctrl + T__               | 查看当前光标下的word的tags                      |

  * :set  tags += tags_file， 添加tags目录
  * ：set tags 查看已有的tags 
  * : tselect 有多个定义时用于选择定义
  * : make xxx.c 直接编译
  * :cc
  * :cn
  * 

* shell环境变量

  __echo $PATH__
  
  ____
  
  # GCC
  
  # Git
  
  Teachable Machine
  
  # Makefile
  
  target:
  
  ​			gcc  <font color='#f00'>-c</font> ####.c -o a.out
  
  ​			添加-c，否则可能会报错
  
  ​			 
  
  
  
  