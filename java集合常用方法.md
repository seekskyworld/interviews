## ArrayList所有方法

`ArrayList` 类实现了 `List` 接口，因此它包含了大量用于操作列表的方法。以下是 `ArrayList` 类中的主要方法：

1. `add(E element)`: 将指定的元素添加到列表的末尾。
2. `add(int index, E element)`: 将指定的元素插入到列表中的指定位置。
3. `addAll(Collection<? extends E> c)`: 将指定 collection 中的所有元素添加到列表的末尾，按照指定 collection 的迭代器返回元素的顺序添加。
4. `addAll(int index, Collection<? extends E> c)`: 将指定 collection 中的所有元素插入到列表中的指定位置，按照指定 collection 的迭代器返回元素的顺序添加。
5. `clear()`: 从列表中移除所有元素。
6. `clone()`: 返回此 `ArrayList` 实例的浅表副本（即元素本身不被复制）。
7. `contains(Object o)`: 如果列表包含指定的元素，则返回 true。
8. `ensureCapacity(int minCapacity)`: 将列表的容量增加到至少等于指定的最小值。
9. `get(int index)`: 返回列表中指定位置的元素。
10. `indexOf(Object o)`: 返回列表中第一次出现指定元素的索引，如果列表不包含该元素，则返回 -1。
11. `isEmpty()`: 如果列表不包含任何元素，则返回 true。
12. `iterator()`: 返回此列表中元素的迭代器（按适当顺序）。
13. `lastIndexOf(Object o)`: 返回列表中最后一次出现指定元素的索引，如果列表不包含该元素，则返回 -1。
14. `listIterator()`: 返回列表中元素的列表迭代器（按适当顺序）。
15. `listIterator(int index)`: 返回列表中元素的列表迭代器（从列表中的指定位置开始）。
16. `remove(int index)`: 移除列表中指定位置的元素。
17. `remove(Object o)`: 移除列表中第一次出现的指定元素（如果存在）。
18. `removeAll(Collection<?> c)`: 从列表中移除包含在指定 collection 中的所有元素。
19. `removeIf(Predicate<? super E> filter)`: 根据给定的谓词（判定条件）移除所有符合条件的元素。
20. `replaceAll(UnaryOperator<E> operator)`: 根据给定的操作符（unary operator）替换列表中的所有元素。
21. `retainAll(Collection<?> c)`: 仅保留列表中包含在指定 collection 中的元素。
22. `set(int index, E element)`: 用指定的元素替换列表中指定位置的元素。
23. `size()`: 返回列表中的元素数。
24. `sort(Comparator<? super E> c)`: 根据指定的比较器（comparator）对列表进行排序。
25. `spliterator()`: 创建一个按适当顺序遍历列表中的元素的 Spliterator。
26. `subList(int fromIndex, int toIndex)`: 返回列表中指定的 fromIndex（包括）和 toIndex（不包括）之间的部分视图。
27. `toArray()`: 返回一个包含列表中所有元素的数组。
28. `toArray(T[] a)`: 返回包含列表中所有元素的数组；返回数组的运行时类型是指定数组的运行时类型。
29. `trimToSize()`: 将列表的容量调整为列表的当前大小。

以上是 `ArrayList` 类的主要方法。这些方法提供了对列表进行添加、移除、查询、遍历、排序等操作的支持。

## HashMap的主要方法

`HashMap` 是 Java 中用于存储键值对的集合类，它基于哈希表实现。以下是 `HashMap` 类的一些主要方法：

1. `put(K key, V value)`: 将指定的键值对映射到 HashMap 中。
2. `get(Object key)`: 返回指定键所映射的值，如果此映射不包含该键的映射，则返回 `null`。
3. getOrDefault()` 方法用于从映射中获取与指定键关联的值。如果该键存在于映射中，则返回与该键关联的值；否则返回指定的默认值。
4. `remove(Object key)`: 移除指定键所映射的键值对。
5. `containsKey(Object key)`: 如果此映射包含指定键的映射关系，则返回 `true`。
6. `containsValue(Object value)`: 如果此映射将一个或多个键映射到指定值，则返回 `true`。
7. `size()`: 返回此映射中的键值对数。
8. `isEmpty()`: 如果此映射未包含键值对，则返回 `true`。
9. `clear()`: 移除此映射中的所有映射关系。
10. `keySet()`: 返回此映射中包含的键的 Set 视图。
11. `values()`: 返回此映射中包含的值的 Collection 视图。
12. `entrySet()`: 返回此映射中包含的映射关系的 Set 视图。
13. `putAll(Map<? extends K, ? extends V> m)`: 将指定映射中的所有映射关系复制到此映射中。
14. `replace(K key, V value)`: 使用指定的值替换指定键的值（如果存在）。
15. `replace(K key, V oldValue, V newValue)`: 使用新值替换给定键的旧值（仅当当前映射到给定键的值等于给定的旧值时才进行替换）。
16. `putIfAbsent(K key, V value)`: 当且仅当指定的键尚未与值关联（或映射到 `null` 时）才将其与给定值关联。
17. `computeIfAbsent(K key, Function<? super K, ? extends V> mappingFunction)`: 如果指定的键尚未与值关联（或映射到 `null` 时），则尝试使用给定的映射函数计算其值。
18. `computeIfPresent(K key, BiFunction<? super K, ? super V, ? extends V> remappingFunction)`: 如果指定键的值存在且不为 `null`，则尝试计算新的映射。
19. `compute(K key, BiFunction<? super K, ? super V, ? extends V> remappingFunction)`: 如果指定的键尚未与值关联（或映射到 `null` 时），则尝试使用给定的映射函数计算其值。
20. `merge(K key, V value, BiFunction<? super V, ? super V, ? extends V> remappingFunction)`: 如果指定的键已经关联了一个非空（非 `null`）的值，则尝试替换该值。
21. `forEach(BiConsumer<? super K, ? super V> action)`: 对 `HashMap` 中的每个键值对执行给定的操作。
22. `replaceAll(BiFunction<? super K, ? super V, ? extends V> function)`: 使用给定的函数对每个键值对执行替换操作。

这些方法提供了对 `HashMap` 中键值对的添加、获取、移除、查询等操作。

### LinkedHashMap和HashMap的方法区别

HashMap和LinkedHashMap除了存储顺序和遍历顺序不同之外，其他方法基本相同。以下是HashMap和LinkedHashMap其他方法的区别：

| 方法                                    | HashMap                                | LinkedHashMap                                          |
| :-------------------------------------- | :------------------------------------- | :----------------------------------------------------- |
| putAll(Map<? extends K, ? extends V> m) | 将指定Map中的所有键值对复制到当前Map中 | 将指定Map中的所有键值对复制到当前Map中，并保持插入顺序 |
| removeEldestEntry()                     | 删除最近最少使用的元素                 | 删除最近最少使用的元素，并保持插入顺序                 |
| clear()                                 | 清空Map                                | 清空Map，并重置插入顺序                                |

## HashSet全部方法

HashSet是Java集合框架中常用的集合类，它继承自AbstractSet类，并实现了Set接口。HashSet中的元素是无序的，并且不允许重复。

HashSet的全部方法如下：

- **add(E e)**：添加元素。如果指定的元素尚不存在，则将其添加到此集合中。

- **addAll(Collection<? extends E> c)**：将指定集合中的所有元素添加到此集合中。

- **clear()**：清空集合。删除集合中的所有元素。

- **clone()**：克隆此集合。

- **contains(Object o)**：判断元素是否存在。返回true表示元素存在，false表示元素不存在。

- **containsAll(Collection<?> c)**：判断指定集合中的所有元素是否都存在于此集合中。

- **equals(Object o)**：比较两个集合是否相等。

- **hashCode()**：返回集合的哈希码。

- **isEmpty()**：判断集合是否为空。返回true表示集合为空，false表示集合非空。

- **iterator()**：返回一个迭代器，用于遍历集合中的元素。

- **remove(Object o)**：删除元素。如果存在，则从该集合中移除指定的元素。

- **removeAll(Collection<?> c)**：删除指定集合中的所有元素。

- **retainAll(Collection<?> c)**：保留指定集合中的所有元素。

- **size()**：返回集合中元素的个数。

- **spliterator()**：返回一个Spliterator，用于并行遍历集合中的元素。

- **toArray()**：将集合转换为数组。

- **toArray(T[] a)**：将集合转换为指定类型的数组。

  

## ArrayDeque的主要方法

ArrayDeque是Java集合框架中常用的**双向队列**类，它继承自AbstractCollection类，并实现了Deque接口。ArrayDeque中的元素是有序的，并且是按照插入顺序排序的。

ArrayDeque的主要方法如下：

`offer()` 方法用于在队尾添加元素，,isEmpty()**：判断队列是否为空。

而 `poll()` 方法用于移除并返回队头元素,pollLast,()删除队列尾部的元素

**1. 添加元素**

- **addFirst(E e)**：将元素添加到队列的头部。
- **addLast(E e)**：将元素添加到队列的尾部。
- **offerFirst(E e)**：将元素添加到队列的头部。如果队列已满，则返回false。
- **offerLast(E e)**：将元素添加到队列的尾部。如果队列已满，则返回false。

**2. 删除元素**

- **removeFirst()**：删除队列头部的元素。
- **removeLast()**：删除队列尾部的元素。
- **pollFirst()**：删除队列头部的元素。如果队列为空，则返回null。
- **pollLast()**：删除队列尾部的元素。如果队列为空，则返回null。

**3. 获取元素**

- **getFirst()**：获取队列头部的元素。
- **getLast()**：获取队列尾部的元素。
- **peekFirst()**：获取队列头部的元素。如果队列为空，则返回null。
- **peekLast()**：获取队列尾部的元素。如果队列为空，则返回null。

**4. 其他方法**

- **isEmpty()**：判断队列是否为空。
- **size()**：返回队列中元素的个数。
- **iterator()**：返回一个迭代器，用于遍历队列中的元素。
- **toArray()**：将队列转换为数组。

## 使用 ArrayDeque 模拟栈

**ArrayDeque** 是 Java 中提供的一个双端队列，它可以高效地在两端进行插入和删除操作。因此，**可以使用 ArrayDeque 模拟栈**，**具体方法如下：**

**1. 入栈**

- 使用 `addLast()` 方法将元素添加到队列的末尾。

Java

```
ArrayDeque<Integer> deque = new ArrayDeque<>();
deque.addLast(1);
deque.addLast(2);
deque.addLast(3);
```

**2. 出栈**

- 使用 `removeLast()` 方法从队列的末尾删除元素。

Java

```
int num = deque.removeLast();
System.out.println(num); // 3
```

**3. 栈顶元素**

- 使用 `peekLast()` 方法获取队列末尾的元素，但不删除它。

Java

```
int num = deque.peekLast();
System.out.println(num); // 2
```

**4. 栈空判断**

- 使用 `isEmpty()` 方法判断队列是否为空。

Java

```
if (deque.isEmpty()) {
    System.out.println("栈空");
}
```

**使用 ArrayDeque 模拟栈的优势:**

- 效率高：ArrayDeque 在两端进行插入和删除操作的效率都很高。
- 线程安全：ArrayDeque 是线程安全的，可以用于多线程环境。

**使用 ArrayDeque 模拟栈的劣势:**

- 不直观：ArrayDeque 是一个双端队列，模拟栈需要额外的方法来实现入栈、出栈等操作。

**总结:**

ArrayDeque 可以用来模拟栈，但需要额外的方法来实现入栈、出栈等操作。如果需要更直观的栈操作，可以使用 `Stack` 类。

## StringBuilder主要方法

StringBuilder是Java集合框架中常用的字符串缓冲区类，它继承自AbstractStringBuilder类，并实现了CharSequence接口。StringBuilder中的字符是可变的，并且可以高效地进行字符串拼接操作。

StringBuilder的主要方法如下：

**1. 追加字符串**

- **append(String str)**：将字符串追加到字符串缓冲区。
- **append(StringBuffer sb)**：将字符串缓冲区追加到字符串缓冲区。
- **append(char[] str)**：将字符数组追加到字符串缓冲区。
- **append(char c)**：将字符追加到字符串缓冲区。
- **append(boolean b)**：将布尔值追加到字符串缓冲区。
- **append(char[] str, int offset, int len)**：将字符数组的一部分追加到字符串缓冲区。
- **append(int i)**：将整数追加到字符串缓冲区。
- **append(long l)**：将长整数追加到字符串缓冲区。
- **append(float f)**：将浮点数追加到字符串缓冲区。
- **append(double d)**：将双精度浮点数追加到字符串缓冲区。
- **append(Object obj)**：将对象追加到字符串缓冲区。

**2. 插入字符串**

- **insert(int index, String str)**：在指定索引处插入字符串。
- **insert(int index, char[] str)**：在指定索引处插入字符数组。
- **insert(int index, char c)**：在指定索引处插入字符。
- **insert(int index, boolean b)**：在指定索引处插入布尔值。
- **insert(int index, int i)**：在指定索引处插入整数。
- **insert(int index, long l)**：在指定索引处插入长整数。
- **insert(int index, float f)**：在指定索引处插入浮点数。
- **insert(int index, double d)**：在指定索引处插入双精度浮点数。
- **insert(int index, Object obj)**：在指定索引处插入对象。

**3. 删除字符串**

- **delete(int start, int end)**：删除指定范围内的字符。
- **deleteCharAt(int index)**：删除指定索引处的字符。

**4. 替换字符串**

- **replace(int start, int end, String str)**：替换指定范围内的字符。

**5. 反转字符串**

- **reverse()**：反转字符串缓冲区中的字符。

**6. 其他方法**

- **length()**：返回字符串缓冲区中的字符个数。
- **capacity()**：返回字符串缓冲区的容量。
- **charAt(int index)**：返回指定索引处的字符。
- **toString()**：返回字符串缓冲区中的字符串。

**7. 转换成String类型**

```java
StringBuilder result = new StringBuilder();
result.toString().trim(); // 将StringBuilder转换为字符串，并去除首尾空格
```



## String字符串转换成int，char数组等方法

**1. String转换成int**

- **使用Integer类的valueOf()方法**

Java

```
String str = "123";
int num = Integer.valueOf(str);
```

请[谨慎使用](https://gemini.google.com/faq#coding)代码。

content_copy

- **使用parseInt()方法**

Java

```
String str = "123";
int num = Integer.parseInt(str);
```

请[谨慎使用](https://gemini.google.com/faq#coding)代码。

content_copy

**2. String转换成char数组**

- **使用toCharArray()方法**

Java

```
String str = "Hello";
char[] chars = str.toCharArray();
```

请[谨慎使用](https://gemini.google.com/faq#coding)代码。

content_copy

- **使用循环**

Java

```
String str = "Hello";
char[] chars = new char[str.length()];
for (int i = 0; i < str.length(); i++) {
    chars[i] = str.charAt(i);
}
```

请[谨慎使用](https://gemini.google.com/faq#coding)代码。

content_copy

**3. String转换成其他类型**

- **使用相应的包装类的valueOf()方法**

Java

```
String str = "true";
boolean b = Boolean.valueOf(str);

String str = "12.34";
double d = Double.valueOf(str);
```

请[谨慎使用](https://gemini.google.com/faq#coding)代码。

content_copy

**4. 注意**

- 在使用Integer.parseInt()方法或Double.parseDouble()方法时，如果字符串不是有效的数字，则会抛出NumberFormatException异常。
- 在使用toCharArray()方法时，返回的char数组是字符串的副本，对原字符串的修改不会影响char数组。

## 集合类型大 PK

在 Java 中，处理数据离不开各种集合类。这里为你列出常用的集合类型及其区别：

![批注 2023-06-16 162835](D:\学习\学习笔记\批注 2023-06-16 162835.jpg)

**1. 存储结构:**

- **Vector (古老系):** 可调整大小的数组，线程安全 (所有方法都同步)。

- **ArrayList:** 可调整大小的数组，非线程安全。

- **LinkedList:** 双向链表，非线程安全。

- TreeSet, TreeMap:

   

  基于红黑树实现排序 (O(log n))。

  - TreeSet: 基于元素的自然顺序或自定义比较器排序，不允许重复元素。
  - TreeMap: 基于键的自然顺序或自定义比较器排序。

- **HashSet:** 基于哈希表实现，平均查找插入时间为 O(1)，无序，不允许重复元素。

- **HashMap:** 基于哈希表实现，平均查找插入时间为 O(1)，无序，允许重复元素。

- **LinkedHashMap:** 兼顾 HashMap 的快速查找和有序性 (按插入顺序)，使用哈希表和双向链表实现。

- **Hashtable (古老系):** 类似于 HashMap，但线程安全 (所有方法都同步)。

**2. 排序:**

- **Vector, ArrayList, LinkedList:** 保持插入顺序。
- **TreeSet, TreeMap:** 元素是排序的。
- **HashSet, HashMap:** 元素是无序的。
- **LinkedHashMap:** 元素按插入顺序排序。

**3. 重复元素:**

- **TreeSet, HashSet:** 不允许重复元素。
- **Vector, ArrayList, LinkedList, HashMap, LinkedHashMap, TreeMap:** 允许重复元素。

**4. 线程安全性:**

- **Vector, Hashtable:** 线程安全。
- **ArrayList, LinkedList, HashSet, HashMap, LinkedHashMap, TreeMap:** 非线程安全。

**5. 使用场景:**

- **Vector (推荐用 ArrayList):** 历史遗留产物，效率不如 ArrayList。
- **ArrayList:** 通用列表，适合频繁随机访问和修改。
- **LinkedList:** 频繁地在链表中间插入/删除元素，不适合随机访问。
- **TreeSet:** 需要排序的元素，且不允许重复。
- **HashSet:** 快速判断元素是否存在，不关心元素顺序 (比如购物车里的商品)。
- **HashMap:** 快速查找键值对，不关心顺序 (比如缓存)。
- **LinkedHashMap:** 需要保持插入顺序，同时还要像 HashMap 一样快速查找 (比如最近打开的文件列表)。
- **TreeMap:** 需要按键排序的键值对 (比如排序后的用户列表)。
- **Hashtable (推荐用带同步的 HashMap):** 类似于 HashMap，但线程安全，效率较低。
- **Properties:** 读写配置文件的键值对。

**总结:**

选择合适的集合类型需要考虑以下因素:

- 是否需要排序？
- 是否允许重复元素？
- 是否需要线程安全？
- jména操作 (查找、插入、删除) 的频率？



## 单列集合，双列集合，数组，零散数据不同的stream流获取方法

单列集合 (Collection)

```java
//直接调用 stream() 方法：
List<String> list = new ArrayList<>();
Stream<String> stream = list.stream(); 

```

双列集合 (Map)

```java
//通过 keySet()、values()、entrySet() 获取键、值、键值对的集合，再调用 stream() 方法：
Map<String, Integer> map = new HashMap<>();
Stream<String> keyStream = map.keySet().stream();
Stream<Integer> valueStream = map.values().stream();
Stream<Map.Entry<String, Integer>> entryStream = map.entrySet().stream();

```

数组

```java
//使用 Arrays 类的静态方法 stream()：
String[] array = {"a", "b", "c"};
Stream<String> stream = Arrays.stream(array);

```

零散数据

```java
//使用 Stream 接口的静态方法 of()：设计初衷是处理任意数量的单个对象，而不是专门处理数组。
Stream<String> stream = Stream.of("x", "y", "z");
//不能获取数组，比如 int[] array = {1, 2, 3};
//Stream.of(array).forEach(s-> System.out.println(s));
//打印的是[I@41629346，因为将整个数组作为一个元素处理了，如果是引用类型数组比如String[]就可以，但不建议
```

steam流常用的处理数据的方法

```java
Stream 流提供了一系列强大的方法来处理数据，下面是一些常用的操作：

//中间操作 (Intermediate Operations)
1. 筛选与切片
filter(Predicate predicate)：过滤元素，只保留满足给定条件的元素。
distinct()：去除重复元素。
limit(long maxSize)：限制 Stream 中元素的最大数量。
skip(long n)：跳过 Stream 中的前 n 个元素。
2. 映射
concat(Stream<? extends T> a, Stream<? extends T> b):接收两个 Stream，类型可以相同，也可以是父子关系,返回一个新的 Stream，包含了两个输入 Stream 中的所有元素。	
map(Function mapper)：将 Stream 中的每个元素转换为另一个元素。
//mapToInt()、mapToDouble()、mapToLong()和.toArray()结合使用
flatMap(Function mapper)：将 Stream 中的每个元素转换为一个 Stream，然后将这些 Stream 合并成一个 Stream。
peek(Consumer action)：对 Stream 中的每个元素执行给定的操作，主要用于调试。
3. 排序
sorted()：对 Stream 中的元素进行自然排序。
sorted(Comparator comparator)：使用指定的 Comparator 对 Stream 中的元素进行排序。
4. 其他
takeWhile(Predicate predicate)：从 Stream 中获取元素，直到遇到不满足给定条件的元素为止。
dropWhile(Predicate predicate)：丢弃 Stream 中的前一部分元素，直到遇到满足给定条件的元素为止。
    
//concat示例
Stream<String> stream1 = Stream.of("a", "b", "c");
Stream<String> stream2 = Stream.of("d", "e", "f");
Stream<String> combinedStream = Stream.concat(stream1, stream2);
combinedStream.forEach(System.out::println); // 输出 a b c d e f，第一个输入 Stream 的元素在前，第二个输入 Stream 的元素在后。

//惰性求值： 中间操作不会立即执行，而是会形成一个操作管道。只有当遇到终止操作时，才会触发整个管道的执行。
//无状态： 中间操作不会修改原始 Stream，而是返回一个新的 Stream。
//链式调用： 中间操作可以链式调用，形成复杂的处理流程。
    
//终止操作 (Terminal Operations)
1. 匹配操作
anyMatch(Predicate predicate)：判断 Stream 中是否有元素满足给定条件。
allMatch(Predicate predicate)：判断 Stream 中是否所有元素都满足给定条件。
noneMatch(Predicate predicate)：判断 Stream 中是否没有元素满足给定条件。
2. 查找操作
findFirst()：返回 Stream 中的第一个元素，如果 Stream 为空则返回 Optional.empty()。
findAny()：返回 Stream 中的任意一个元素，如果 Stream 为空则返回 Optional.empty()。
3. 归约操作
reduce(T identity, BinaryOperator<T> accumulator)：从一个初始值开始，将 Stream 中的元素逐个与累加器函数的结果进行累积，最终得到一个值。
reduce(BinaryOperator<T> accumulator)：与上面的方法类似，但没有初始值，如果 Stream 为空则返回 Optional.empty()。
collect(Collector collector)：使用 Collector 将 Stream 中的元素收集到一个结果容器中，例如 List、Set、Map 等。
 //.collect(Collectors.toList()),Collectors.toSet(),.toMap(),依次为lsit和set和map，
// 和.toMap()不同，.groupingBy()将相同组的元素收集到一个 List 中
//Collectors.joining()：将 Stream 中的字符串元素连接成一个字符串。
//Collectors.counting()：计算 Stream 中的元素个数，
4. 迭代操作
forEach(Consumer action)：对 Stream 中的每个元素执行给定的操作。
forEachOrdered(Consumer action)：与 forEach 类似，但保证按照元素的 encounter order 执行操作。
5. 数值操作
count()：返回 Stream 中的元素个数。
max(Comparator comparator)：返回 Stream 中的最大值，如果 Stream 为空则返回 Optional.empty()。
min(Comparator comparator)：返回 Stream 中的最小值，如果 Stream 为空则返回 Optional.empty()。
sum()：返回 Stream 中所有元素的和（仅适用于数值类型的 Stream）。
average()：返回 Stream 中所有元素的平均值（仅适用于数值类型的 Stream）。
6. 其他操作
toArray()：将 Stream 中的元素收集到一个数组中。
```

```java
示例
List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6);

// 筛选出偶数，乘以2，去重，求和
int sum = numbers.stream()
    .filter(n -> n % 2 == 0)
    .map(n -> n * 2)
    .distinct()
    .reduce(0, Integer::sum);
System.out.println(sum); // 输出 12

// 筛选中文第二个字符为无，长度为3的
//对于中文字符串，一个中文字符通常占用两个字符位置，因此 charAt(1) 获取到的可能不是您期望的字符。如果需要处理中文字符串，建议使用 codePointAt(1) 获取字符的 Unicode 编码点。
List<String> list = new ArrayList<>();
        Collections.addAll(list,"张无忌","晓无","周芷若","张三丰","张铁");
        list.stream().filter(name -> name.length() >= 2 && name.codePointAt(1) == '无').filter(name -> name.length()==3).forEach(data -> System.out.println(data));// 输出 张无忌

//collect示例
List<String> list = new ArrayList<>();
Collections.addAll(list,"zhangsan,23","lisi,24","wangwu,25");
Map<String, String> map = list.stream().filter(data -> 24 <= Integer.parseInt(data.split(",")[1])).collect(Collectors.toMap(data -> data.split(",")[0], data -> data.split(",")[1]));//键值对一一对应，输出 {lisi=[24], wangwu=[25]}

List<String> list = new ArrayList<>();
        Collections.addAll(list,"zhangsan,23","lisi,24","wangwu,25","lisi,26");
        Map<String, List<String>> collect = list.stream()
                .filter(data -> 24 <= Integer.parseInt(data.split(",")[1]))
                .collect(Collectors.groupingBy(
                        data -> data.split(",")[0],  // 提取姓名作为键
                        Collectors.mapping(           // 使用 mapping 收集器
                                data -> data.split(",")[1], // 提取年龄
                                Collectors.toList()       // 收集到 List 中
                        )
                ));			//重复的值放进集合， 输出 {lisi=[24, 26], wangwu=[25]}

//现在有两个ArrayList集合,分别存储6名男演员的名字和年龄以及6名女演员的名字和年龄。姓名和年龄中间用逗号隔开。
        // 比如：张三，23    要求完成如下的操作：
        // 1,男演员只要名字为3个字的前两人
        // 2,女演员只要姓杨的，并且不要第一个
        // 3.把过滤后的男演员姓名和女演员姓名合并到一起
        // 4,将上一步的演员姓名封装成Actor对象。
        // 5,将所有的演员对象都保存到List集合中。
        // 备注:演员类Actor,属性有: name, age
        List<String> list1 = new ArrayList<>();
        Collections.addAll(list1,"蔡坤坤,24","叶齁咸,23","刘不甜,22","吴签,24","谷嘉,30","肖梁梁,27");
        List<String> list2 = new ArrayList<>();
        Collections.addAll(list2,"赵小颖,35","杨颖,36","高元元,43","张天天,31","刘诗,35","杨小幂,33");
        Stream<String> limit = list1.stream().filter(s -> s.split(",")[0].length() == 3).limit(2);
        Stream<String> skip = list2.stream().filter(s -> (s.split(",")[0]).startsWith("杨")).skip(1);        //中英文逗号和startsWith问题
        List<Actor> collect = Stream.concat(limit, skip).map(s -> new Actor(s.split(",")[0], Integer.parseInt(s.split(",")[1]))).collect(Collectors.toList());
        System.out.println(collect);

```

## 基础类型和包装

| 基础类型 | 包装类（首字母大写） |
| -------- | -------------------- |
| byte     | Byte                 |
| short    | Short                |
| int      | Integer              |
| long     | Long                 |
| float    | Float                |
| double   | Double               |
| char     | Character            |
| boolean  | Boolean              |

### [自动装箱与拆箱了解吗？原理是什么？](https://javaguide.cn/java/basis/java-basic-questions-01.html#自动装箱与拆箱了解吗-原理是什么)

**什么是自动拆装箱？**

- **装箱**：将基本类型用它们对应的引用类型包装起来；
- **拆箱**：将包装类型转换为基本数据类型；

从字节码中，我们发现装箱其实就是调用了 包装类的`valueOf()`方法，拆箱其实就是调用了 `xxxValue()`方法。

因此，

- `Integer i = 10` 等价于 `Integer i = Integer.valueOf(10)`
- `int n = i` 等价于 `int n = i.intValue()`;

注意：如果频繁拆装箱的话，也会严重影响系统的性能。我们应该尽量避免不必要的拆装箱操作。

### **BigInteger:**

- **算术运算：**
  - `add(BigInteger val)`: 加法
  - `subtract(BigInteger val)`: 减法
  - `multiply(BigInteger val)`: 乘法
  - `divide(BigInteger val)`: 除法
  - `remainder(BigInteger val)`: 取余
  - `pow(int exponent)`: 幂运算
  - `negate()`: 取相反数
  - `abs()`: 取绝对值
- **比较：**
  - `compareTo(BigInteger val)`: 比较大小 (-1, 0, 1)
  - `equals(Object x)`: 判断是否相等
  - `min(BigInteger val)`: 取较小值
  - `max(BigInteger val)`: 取较大值
- **其他：**
  - `valueOf(long val)`: 将 long 值转换为 BigInteger
  - `toString()`: 转换为字符串

### **BigDecimal:**

- **算术运算：**

  - `add(BigDecimal val)`: 加法
  - `subtract(BigDecimal val)`: 减法
  - `multiply(BigDecimal val)`: 乘法
  - `divide(BigDecimal val, int roundingMode)`: 除法 (需要指定舍入模式)
  - `remainder(BigDecimal val)`: 取余
  - `pow(int n)`: 幂运算
  - `negate()`: 取相反数
  - `abs()`: 取绝对值

- **比较：**

  - `compareTo(BigDecimal val)`: 比较大小 (-1, 0, 1)
  - `equals(Object x)`: 判断是否相等
  - `min(BigDecimal val)`: 取较小值
  - `max(BigDecimal val)`: 取较大值

- **舍入和格式化：**

  - `setScale(int newScale, int roundingMode)`: 设置小数位数和舍入模式
  - `round(MathContext mc)`: 按照指定 MathContext 舍入
  - `toString()`: 转换为字符串
  - `toPlainString()`: 转换为不带指数的字符串

- **其他：**

  - `valueOf(double val)`: 将 double 值转换为 BigDecimal (注意精度问题)
  - `valueOf(long val)`: 将 long 值转换为 BigDecimal
  - `valueOf(long unscaledVal, int scale)`: 将 unscaledVal / 10^scale 转换为 BigDecimal

  ```java
  //示例
  BigInteger a = BigInteger.valueOf(123456789);
  BigInteger b = BigInteger.valueOf(987654321);
  BigInteger c = a.multiply(b); // 乘法
  
  BigDecimal x = BigDecimal.valueOf(3.14159);
  BigDecimal y = BigDecimal.valueOf(2.71828);
  BigDecimal z = x.divide(y, 5, RoundingMode.HALF_UP); // 除法，保留5位小数，四舍五入
  
  ```

  **注意：**

  - `BigDecimal` 的除法需要指定舍入模式，以避免无限循环小数的情况。
  - 由于浮点数精度问题，直接使用 `BigDecimal.valueOf(double val)` 可能会导致精度损失，建议使用字符串构造函数 `new BigDecimal("3.14159")`。