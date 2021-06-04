## HashMap

#### put(key,value)方法?



```java
static final int hash(Object key) {
        int h;     
        return (key == null) ? 0 : (h = key.hashCode()) ^ ();
    } 
/*
	三目表达式：表达式 ? 1:2;  //表达式true，返回1；否则返回2
	^：是异或；h >>> 16 : >>> 是无符号右移，取整数，左边用0代替
*/
```

