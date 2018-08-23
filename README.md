#上传github过程
```bash
# 使用Git上传项目代码到github
   https://blog.csdn.net/top_code/article/details/50241999
# Git使用设置ssh key 
   http://yuzhouxiner.iteye.com/blog/2258790
# git 上传文件到仓库上提示：origin does not to be a git repository
    https://blog.csdn.net/dream_follower/article/details/53907217
```
# JavaSript-Plugin
##星级评分插件
```bash 
    这是我个人学习插件的过程中源码解读过程
      ##1.理解jquery的$.extend()、$.fn和$.fn.extend()
        ##https://blog.csdn.net/dviewer/article/details/49934925
          jQuery.fn.extend(object);	
          对jQuery.prototype进得扩展，就是为jQuery类添加“成员函数”。jQuery类的实例可以使用这个“成员函数”,
          比如我们要开发一个星级评分插件,可以这么做
          jQuery.fn.extend({
            ratingStars:function(){}
          })
          等价与
            jQuery.prototype.extend(ratingStars)
          还等价于：
            jQuery.fn.ratingStars = function( options ) {	}
          //调用时：
            $(".rating-stars").ratingStars(ratingOptions)
```
