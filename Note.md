# 各语言在算法中的应用

## 1. java

### 数学函数

```java
//Math 库下
static Object abs(Object a)//绝对值
static double ceil(double a)//向上取整
static double floor(double a)//向下取整
static Object min(Object a, Object b)//最小值
static Object max(Object a, Object b)//最大值
static double pow(double a, double b)//返回a的b次幂
static double random()//随机函数，生成一个 [0.0,1.0) 的小数
static double sqrt(double a)//求平方根
```

## Arrays

```java
//数组排序
static void sort(Object[] a)
static void sort(Object[] a, int fromIndex, int toIndex)
```

```java
//用于一维数组、二维数组的初始化或者填充
static void fill(Object[] a, int fromIndex, int tolndex, Object val);
static void fill(Object[] a, Object val)// 下标形式遵循左闭右开
//exam:
     boolean[] a1 = new boolean[5];
     Arrays.fill( a1,true );
     // 结果 a1[] = {true,true,true,true,true};

     boolean[] a1 = new boolean[5];
     Arrays.fill( a1,true );
     Arrays.fill( a1,3,4,false);
     //结果 a1[] = {true,true,true,false,true};
```

```java
//二分搜索，返回key值的下标(索引)
static int binarySearch(Object[] a, Object key)
static int binarySearch(Object[] a, int fromIndex, int tolndex, Object key)
// 下标形式遵循左闭右开
```

```java
//拷贝一个数组
static Object[] copyOf(Object[] original, int newLength)
//exam:
    int[] a = {0,1,2,3,4,5};
    int[] b = Arrays.copyOf(a,3);//{0,1,2}
static Object[] copyOfRange(Object[] original, int from, int to)
//exam:
    int[] a = {0,1,2,3,4,5};
    int[] b = Arrays.copyOfRange(a,2,5);//{2,3,4}
```

```java
//判断两个同类型数组是否相等
static boolean equals(Object[] a, Object[] b) 
```

```java
//数组转成字符串
static String toString(Object[] a)
int[] a = {0,1,2,3,4,5};
String s = Arrays.toString(a);// s = "[0, 1, 2, 3, 4, 5]";
```

## String

```java
char charAt(int index)//下标访问 ，有越界检查
int codePointAt(int index)//在字符串的指定索引处返回字符的Unicode值
int codePointBefore(int index)//返回指定下标前一个字符的Unicode值，下标从1开始(0将越界产生错误)
String concat(String str)//将指定字符串连接到改字符串尾部，当然可以直接用 + 

```

