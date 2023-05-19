# break与continue

## break
结束控制语句

```java
public class BreakStatement {
    public static void main(String[] args) {

        for (int i = 0; i < 10; i++) {
            if (i == 5) {
                break;
            }

            System.out.println(i);
        }
    }
}
```
结果
<p>通过结果可以看出,循环到达5的时候就直接结束程序</p>

```
    0
    1
    2
    3
    4
```

## continue
跳过本次，继续下一次

```java
public class ContinueStatement {
    public static void main(String[] args) {
        for (int i = 0; i < 10; i++) {
            if (i == 5) {
                continue;
            }
            System.out.println(i);
        }
    }
}
```
结果
<p>通过结果可以看出，当循环程序到达5的时候，会跳过这次循环，执行下一次循环</p>

```
    0
    1
    2
    3
    4
    6
    7
    8
    9
```