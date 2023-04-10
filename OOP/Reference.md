# Main
## class StringBuilder implements CharSequence
### constructor
- public StringBuilder(): leere charSequenz
- public StringBuilder(String s): s.toCharArray als initiale CharSequenz
#### methoden
- append(charlike c), reverse(), deleteCharAt(int index), insert(int offset, CharLike c), replace(int start, int end, String s)} -> this
- length() -> int,
- toString() -> String, substring(int start) -> String, substring(int start, int end) -> String
- indexOf(String s), indexOf(String s, int from), lastIndexOf(String s), lastIndexOf(String s), lastIndexOf(String s, int before)} -> int
- setCharAt(int index) -> void
- 
- delete(int start,int end) -> this: löscht die Einträge von start bis einschließlich end-1. Länge der Gelöschten Zeichenkette: end-start
# java.util
## interface Collection\<E\> extends Iterable
### methoden
- {add(E e), addAll(Collection\<? extends E\> c), contains(Object o), isEmpty(), containsAll(Collection\<? extends E\> c)} -> bool, 
- clear() -> void, size() -> int, toArray() -> Object[], toArray(T\[\] t) -> \<T\> T[]
- remove(Object o) -> bool: removes the first entry of o in this
- removeAll(Collection\<? extends E\> c) -> bool: removes the first entry for all E in c
## interface List\<E\> extends Collection
### methoden
- {get(int i), remove(int i), set(int i, E element)} -> E, subList(int from, int toExcl) -> List\<E\>
## abstract class AbstracList\<E\> implements List
## class Vector\<E\> extends AbstractList
### constructor
- Vector(), Vector(Collection\<? extends E\> c), Vector(int initCapa), Vector(int initCapa, int incr)
### methoden
- clone() -> Object: returns a hardcoppy
- {indexOf(Obj o), indexOf(Obj o, int index), lastIndexOf(Obj o), lastIndexOf(Obj o, int index)} -> int, removeRange(int from, int toExcl) -> void
## class Stack\<E\> implements Vector
### constructor
- Stack()
### methoden 
- empty() -> bool, peek() -> E, pop() -> E, push(E item), search(Object o)
## interface Map\<K, V\>
### methoden
- clear() -> void, putAll(Map\<K, V\> map) -> void
- {containsKey(Object key), containsValue(Object value),  isEmpty(), remove(Object key), remove(Object key, Value val)} -> bool
- {get(Object key), getOrDefault(Object key, V defaultValue), putIfAbsent(K key, V value), put(K key, V value) }-> V, 
- keySet() -> Set\<K\>
- values() -> Collection\<V\>
- {compute(K key, BiFunction\<? super K, ? super V, ? extends V\> remap), computeIfPresent(K key, BiFunction\<? super K, ? super V, ? extends V\> remap)} -> V: maps the element v at Position key (if present and non-null) onto the value of remap.apply(key, v) (or null if not present)
- computeIfAbsent(K key, Function\<? super K, ? extends V\> map) -> V: maps the element at key to map.apply(key) if there exists no mapping for key
- merge(K key, V value, BiFunction\<? super V, ? super V, ? extends V\> remap) -> V: maps Key to V if key is emptymapped, maps Key to remap.apply(V, this.get(key)) otherwise. Unmaps key if remap produces null
- replace(K key, V val), replace(K key, V oldVal, V val) -> bool: maps key to val only if key is mapped (and this.get(key).equals(oldVal))
- replaceAll(BiFunction\<? super K, ? super V, ? extends V\> func) -> void: maps k -> func.apply(k, this.get(k)) for all keys currently mapped
## class AbstractMap\<K, V\> implements Map
## class HashMap\<K, V\> extends AbstractMap
package java.util
### descr:
maps the values by using K.hashValue() as a comperisonTool
### constructor:
- HashMap(), HashMap(int initialCapacity), HashMap(Map\<? extends K, ? extends V\> m)
## interface SortedMap\<Comparable K, V\> extends Map
### methoden
- firstKey(), lastKey() -> K
- headMap(K key), tailMap(K key) -> SortedMap\<K, V\>: returns a Map with all the values less then(greater then or equal to) key
- subMap(K from, K to) -> SortedMap\<K, V\>: returns a subMap starting at from and ending before to
## interface NavigableMap\<K, V\> extends SortedMap
### methoden
- ceilingKey(K key) -> K, ceilingEntry(K key) -> V: returns the smallest Key(or mapped Value) greater then or equal to key
- floorKey(K key) -> K, floorEntry(K key) -> V: analog to ceiling
- descendingKeySet() -> NavigableSet\<K\>, descendingMap() -> NavigableMap\<K, V\>: reverse ordered set/ map
- firstEntry() -> V, lastEntry() -> V, navigableKeySet() -> NavigableSet\<K, V\>
- higherEntry(K key) -> V, higherKey(K key) -> K, lowerEntry(K key) -> V, lowerKey(K key): returns the first entry/ key greater then(less then or equal) key
## class TreeMap\<Comparable K, V\> extends AbstractMap implements NavigableMap
### descr:
a sorted version of a map
### constructor:
- TreeMap(), TreeMap(Map\<? extends K, ? extends V\> m), TreeMap(SortedMap\<? extends K, ? extends V\>)
## interface Set\<E\> extends Collection
### descr:
ensures that every Element is contained only once
## class AbstractSet\<E\> implements Set
## class HashSet\<E\> extends AbstractSet
### constructor
- HashSet(), HashSet(int initialCapacity), HashSet(Collection\<? extends E\>)
## interface SortedSet\<Comparable E\> extends Set
### methoden
- first() -> E, last() -> E
- headSet(E e) -> SortedSet\<E\>, tailSet(E e) -> SortedSet\<E\>: returned ein Set mit allen Elementen kleiner(größer gleich) e
- subSet(E from, E to) -> SortedSet\<E\>: returned ein Set mit allen Elementen größer gleich from und kleiner to
## interface NavigableSet\<Comparable E\> extends SortedSet
### methoden
- ceiling(E e) -> E, floor(E e) -> E: returned das kleinste (größte) Element größer gleich (kleiner gleich) e
- higher(E e) -> E, lower(E e) -> E: returned das kleinste (größte) Element kleiner (größer) e
## interface TreeSet\<Comparable E\> extends Set implements NavigableSet
### descr:
A sorted set implementation
### constructor
- TreeSet(), TreeSet(Collection\<? extends E\>), TreeSet()
# java.util.function
## interface Function\<T, R\>
### methods
- apply(T t) -> R
- \<V\> compose(Function\<? super V, ? extends T\> before) -> Function\<V, R\>: returns a function f of the type: $f: V \to R, x \onto$ this(before(x))
- \<V\> andThen(Function\<? super R, ? extends V\> after) -> Function\<T, V\>: returns a function f of the type: $f: T \to V, x \onto$ after(this(x))
## interface BiFunction\<T, U, R\>
### methods
- apply(T t, U u) -> R
- \<V\> andThen(Function\<? super R, ? extends V\> after) -> BiFunction\<T, U, V\>: returns a function f of the type: $f: (T, U) \to V, (x,y) \onto$ after(this(x,y))
