---
修改PHP时区问题
---
当你在使用PHP操纵文件时间的时候，你会发现时间和我们并不相同，这是因为PHP的默认时间为格林威治标准时间，所以和我们的时间是有差别的，下面给出了两种可以修改时区的方法哦：

>1.直接在你的php代码前部加上这样一句：
>date_default_timezone_set('Aisa/Beijing');

>2.如果你想一劳永逸的话，就要修改你的`php ini`了，如果你使用的是wampsever，首先左键找到并打开`php ini`，接下来`ctrl+F`输入timezone快速找到，并将之前的UFC修改为PRC即可，重启你的wampsever，你会发现完美的解决了时区问题。

![](http://i.imgur.com/tcv3qso.jpg)

----------

![](http://i.imgur.com/7Vn9hpL.jpg)

----------
![](http://i.imgur.com/peTZowA.jpg)

