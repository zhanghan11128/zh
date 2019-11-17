一、实验目的
掌握字符串String及其方法的使用
掌握异常处理结构
二、实验内容
内容：利用已学的字符串处理知识编程完成《长恨歌》古诗的整理对齐工作，写出功能函数，并运行。达到如下功能：

1.	每7个汉字加入一个标点符号，奇数时加“，”，偶数时加“。”
2.	允许提供输入参数，统计古诗中某个字或词出现的次数
3.	考虑操作中可能出现的异常，在程序中设计异常处理程序
三、流程图
![image](https://github.com/zhanghan11128/zh/blob/master/zh.jpg)
四、核心代码
1.用for循环每7个字添加一个逗号，每14字添加一个句号和换行符 
for(int i=0;i<s.length()/7;i++) {
        str.append(str.substring(7*i, 7*(i+1)));
       
        if((i+1)%2!=0) {
         str.append(",");
        }
        else {
         str.append("。").append("\n");
        }
       }
	System.out.println(str);
2．对比字符是否相等，输出相同字符数目
 StringTokenizer a = new StringTokenizer(s,c);
    int number = a.countTokens();
    while(a.hasMoreTokens()) 
    {
     String k = a.nextToken();
    }
    if(c.equals("行"))
    {
     number = number;
    }
    else if(c.equals("汉")) 
    {
     number = number;
    }
    else 
    {
     number=number -1;
    }
     g = number;
   System.out.println("所查字 “"+c+"”出现过："+g+"次。");
五、实验结果
![image](https://github.com/zhanghan11128/zh/blob/master/1111.png)
六、实验感想
实验过程中经常遇到不会的问题，这时可以选择向老师和同学求助，实在不行还可以上网搜索解决方案。在写代码的时候经常会出现小细节的错误，这提醒了我在以后的学习中要更加认真仔细，对每一行代码都要认真的阅读，进行检查和完善。养成这个好习惯将对我以后的学习有更多的好处。
