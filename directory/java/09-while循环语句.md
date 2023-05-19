## while循环
- while循环语句用于重复执行一段代码，只要为真 (true)就会重复执行。

```java
while (布尔表达式) {
    // 执行代码块
}
```

### 例子1
计算1-10之间的和

```java
public class WhileStatement {
    public static void main(String[] args) {
        int i = 1;
        int sum = 0;

        while (i <= 10) {
            sum += i;
            i++;
        }

        System.out.println("sum = " + sum);
    }
}
```
首先该程序定义一个int类型变量i为初始值1，定义int类型sum存储和，while当中的布尔表达式是 i <= 10，通过sum += i 将每个数都进行累加，i++ 每执行一次，对i进行加1操作。
结果:
```
sum = 55
```

### 例子2
打印九九乘法表

```java
public class MultiplicationTable {
    public static void main(String[] args) {
        int i = 1; // 定义外层初始值
        while (i <= 9) {    
            int j = 1;  // 定义内层初始化 
            while (j <= i) {
                System.out.print(i+"x"+j +"=" +i*j + "\t");
                j++;    // 每执行一次，对内层进行加1
            }
            // 内层循环结束，换行
            System.out.println();
            i++; // 外层加1
        }
    }
}
```

结果:
```
1x1=1	
2x1=2	2x2=4	
3x1=3	3x2=6	3x3=9	
4x1=4	4x2=8	4x3=12	4x4=16	
5x1=5	5x2=10	5x3=15	5x4=20	5x5=25	
6x1=6	6x2=12	6x3=18	6x4=24	6x5=30	6x6=36	
7x1=7	7x2=14	7x3=21	7x4=28	7x5=35	7x6=42	7x7=49	
8x1=8	8x2=16	8x3=24	8x4=32	8x5=40	8x6=48	8x7=56	8x8=64	
9x1=9	9x2=18	9x3=27	9x4=36	9x5=45	9x6=54	9x7=63	9x8=72	9x9=81	
```

## <a href="">下一节 do..while循环语句</a>