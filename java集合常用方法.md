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