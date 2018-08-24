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
          调用时：
            $(".rating-stars").ratingStars(ratingOptions)
     ##2.jQuery.extend 函数使用详解
         extend(dest,src1,src2,src3...);
           它的含义是将src1,src2,src3...合并到dest中,返回值为合并后的dest,由此可以看出该方法合并后，是修改了dest的结构的。如果想要得到合并的结果却又            不想修改dest的结构，可以如下使用
         举例：var settings = $.extend( {}, defaults, options );
         上述的extend方法原型中的dest参数是可以省略的，如果省略了，则该方法就只能有一个src参数，而且是将该src合并到调用extend方法的对象中去
    ##3.$.each(arr,function(index,element){})
    ##4.jQuery中this与$(this)的区别总结
      this其实是一个html 元素, $(this)是一个JQuery对象。  
      学习网址： https://blog.csdn.net/BaiHuaXiu123/article/details/51959955
```
