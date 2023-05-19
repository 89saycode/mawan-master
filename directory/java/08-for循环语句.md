# 循环
## 什么是循环?
循环就是在满足条件的情况下，重复的去执行某段代码块。

### for循环
- 初始值: 一个变量的起始值
- 循环条件: 在这个变量满足什么的条件的情况下进行循环。
- 步长值: 每循环一次，初始值 +几位或 -几位

```java
    for (初始值;循环条件;步长值) {
        代码块;
    }
```

```java
public class ForLoopExample {
   public static void main(String[] args) {
      for(int i = 0; i < 5; i++) {
         System.out.println("i = " + i);
      }
   }
}
在for循环中，int i = 0表示循环计数器初始值为0；i < 5表示循环条件，即当计数器小于5时继续循环；i++表示每次循环结束后计数器加1。System.out.println()用于将计数器的值输出到控制台。

```
结果
```
i = 0
i = 1
i = 2
i = 3
i = 4
```

### 练习1
输出5-15之间的数字


```java
public class ForPracticeOne {
    public static void main(String[] args) {
        for (int i = 5; i < 16; i++) {
            System.out.println("i = " + i);
        }
    }
}
```
结果
```
i = 5
i = 6
i = 7
i = 8
i = 9
i = 10
i = 11
i = 12
i = 13
i = 14
i = 15

```

### 练习2
倒序输出0-5之间的数,输出格式
```
4
3
2
1
0
```
Java代码

```java
public class ForPracticeTwo {
    public static void main(String[] args) {

        for (int i = 4; i >= 0; i--) {
            System.out.println(i);
        }
    }
}
```
结果
```
4
3
2
1
0
```
其实这和正序输出没太多的不同，只不过是调整了初始值为4，循环条件大于等于0，步长值-1

### 练习3
求数字0-5之间的和,不包含数字5。
输出格式:
```
和为: 100
```

```java
public class ForPracticeThree {
    public static void main(String[] args) {

        // 存储和的结果值
        int sum = 0;

        for (int i = 0; i < 5; i++) {
            // 每循环一次，将i的值 加赋到sum结果值当中
            sum += i;
        }
        System.out.println("和为: " + sum);
    }
}
```
结果

```
和为: 10
```
### 练习4
求1-100之间的偶数和

Java代码

```java
public class ForPracticeFour {
    public static void main(String[] args) {

        int sum = 0;

        for (int i = 0; i < 100; i+=2) {
            sum += i;
        }

        System.out.println("偶数和为: " + sum);
    }
}
```
结果

```
偶数和为: 2450
```

## <a href="">下一节 while循环语句</a>