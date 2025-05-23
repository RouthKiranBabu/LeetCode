# ✅ Java Program 
## To Print All LinkedList Methods:
```java
package Package;

import java.lang.reflect.Method;
import java.util.LinkedList;
public class firstClass {
	public static void main(String[] args) {
		// Get the LinkedList class
	        Class<?> linkedListClass = LinkedList.class;
	        // Get all methods of LinkedList class
	        Method[] methods = linkedListClass.getDeclaredMethods();
	        System.out.println("Methods available in java.util.LinkedList:\n");
	        int i = 0;
	        for (Method method : methods) {
	        	i += 1;
	            System.out.print(i + ". " + method.getName() + " ");
	            if (i % 5 == 0) System.out.println();
	        }
	        System.out.println("\nTotal number of methods: " + methods.length);
	}
}
```
## Output
```bash
Methods available in java.util.LinkedList:

1. remove 2. remove 3. remove 4. size 5. get 
6. clone 7. indexOf 8. clear 9. lastIndexOf 10. add 
11. add 12. toArray 13. toArray 14. contains 15. spliterator 
16. addAll 17. addAll 18. set 19. readObject 20. writeObject 
21. peek 22. node 23. outOfBoundsMsg 24. getFirst 25. getLast 
26. element 27. addFirst 28. addLast 29. removeFirst 30. removeLast 
31. listIterator 32. reversed 33. reversed 34. reversed 35. reversed 
36. poll 37. push 38. pop 39. pollFirst 40. pollLast 
41. offerLast 42. peekFirst 43. removeFirstOccurrence 44. offerFirst 45. peekLast 
46. removeLastOccurrence 47. offer 48. descendingIterator 49. unlink 50. unlinkFirst 
51. unlinkLast 52. linkFirst 53. linkLast 54. checkPositionIndex 55. checkElementIndex 
56. linkBefore 57. isElementIndex 58. isPositionIndex 59. superClone 
Total number of methods: 59
```
## To Print All Vector Methods:
```java
package Package;
import java.lang.reflect.Method;
import java.util.Vector;
public class firstClass {
	public static void main(String[] args) {
		// Get the Vector class
	        Class<?> vectorClass = Vector.class;
	        // Get all declared methods in Vector class
	        Method[] methods = vectorClass.getDeclaredMethods();
	        System.out.println("Methods available in java.util.Vector:\n");
	        for (Method method : methods) {
	            // Print method name with parameter types
	            System.out.print(method.getName() + "(");
	            Class<?>[] parameterTypes = method.getParameterTypes();
	            for (int i = 0; i < parameterTypes.length; i++) {
	                System.out.print(parameterTypes[i].getSimpleName());
	                if (i < parameterTypes.length - 1) {
	                    System.out.print(", ");
	                }
	            }
	            System.out.println(")");
	        }
	}
}

```
## Output

<details>
  <summary>Show</summary>
	
```bash
Methods available in java.util.Vector:

remove(int)
remove(Object)
size()
get(int)
equals(Object)
toString()
hashCode()
clone()
sort(Comparator)
indexOf(Object)
indexOf(Object, int)
clear()
lastIndexOf(Object)
lastIndexOf(Object, int)
isEmpty()
replaceAll(UnaryOperator)
add(Object, Object[], int)
add(Object)
add(int, Object)
subList(int, int)
toArray()
toArray(Object[])
iterator()
contains(Object)
elements()
spliterator()
addAll(int, Collection)
addAll(Collection)
set(int, Object)
readObject(ObjectInputStream)
writeObject(ObjectOutputStream)
forEach(Consumer)
capacity()
ensureCapacity(int)
trimToSize()
elementData(int)
grow()
grow(int)
shiftTailOverGap(Object[], int, int)
elementAt(int)
elementAt(Object[], int)
removeIf(Predicate)
nBits(int)
setBit(long[], int)
isClear(long[], int)
removeRange(int, int)
removeAll(Collection)
retainAll(Collection)
listIterator(int)
listIterator()
checkInvariants()
containsAll(Collection)
bulkRemove(Predicate)
lambda$retainAll$1(Collection, Object)
lambda$removeAll$0(Collection, Object)
setSize(int)
copyInto(Object[])
removeElementAt(int)
removeElement(Object)
insertElementAt(Object, int)
removeAllElements()
firstElement()
lastElement()
setElementAt(Object, int)
addElement(Object)
```
</details>

## To Print All Stack Methods:
```java
package Package;
import java.lang.reflect.Method;
import java.util.Stack;
public class firstClass {
	public static void main(String[] args) {
		// Get the Stack class object
	        Class<?> stackClass = Stack.class;
	        // Get all methods of Stack (inherited and declared)
	        Method[] methods = stackClass.getMethods();
	        System.out.println("Methods available in java.util.Stack:");
	        int i = 1;
	        for (Method method : methods) {
	            System.out.print(i + ". " + method.getName() + " ");
	            if (i % 5 == 0) System.out.println();
	            i += 1;
	        }
	}
}
```
## Output
```bash
Methods available in java.util.Stack:
1. empty 2. peek 3. search 4. push 5. pop 
6. addElement 7. removeElementAt 8. removeElement 9. insertElementAt 10. removeAllElements 
11. firstElement 12. lastElement 13. setElementAt 14. remove 15. remove 
16. size 17. get 18. equals 19. toString 20. hashCode 
21. clone 22. sort 23. indexOf 24. indexOf 25. clear 
26. lastIndexOf 27. lastIndexOf 28. isEmpty 29. replaceAll 30. add 
31. add 32. subList 33. toArray 34. toArray 35. iterator 
36. contains 37. elements 38. spliterator 39. addAll 40. addAll 
41. set 42. forEach 43. capacity 44. ensureCapacity 45. trimToSize 
46. elementAt 47. removeIf 48. removeAll 49. retainAll 50. listIterator 
51. listIterator 52. containsAll 53. setSize 54. copyInto 55. getClass 
56. notify 57. notifyAll 58. wait 59. wait 60. wait 
61. toArray 62. stream 63. parallelStream 64. getFirst 65. getLast 
66. addFirst 67. addLast 68. removeFirst 69. removeLast 70. reversed 
71. reversed 
```
## To Print All ArrayList Methods:
```java
package Package;
import java.util.ArrayList;
import java.lang.reflect.Method;
public class firstClass {
	public static void main(String[] args) {
		Class<?> arrayListClass = ArrayList.class;
	        // Get all declared methods
	        Method[] methods = arrayListClass.getDeclaredMethods();
	        System.out.println("All methods of ArrayList:\n");
	        int i = 1;
	        for (Method method : methods) {
	            System.out.print(i + ". " + method.getName() + ", ");
	            i += 1;
	            if (i % 10 == 0) System.out.println();
	        }
	}
}
```
## Output
```bash
All methods of ArrayList:

1. remove, 2. remove, 3. size, 4. get, 5. equals, 6. hashCode, 7. clone, 8. sort, 9. indexOf, 
10. clear, 11. lastIndexOf, 12. isEmpty, 13. replaceAll, 14. add, 15. add, 16. add, 17. subList, 18. toArray, 19. toArray, 
20. iterator, 21. contains, 22. spliterator, 23. addAll, 24. addAll, 25. set, 26. readObject, 27. writeObject, 28. forEach, 29. ensureCapacity, 
30. trimToSize, 31. elementData, 32. grow, 33. grow, 34. indexOfRange, 35. lastIndexOfRange, 36. rangeCheckForAdd, 37. fastRemove, 38. equalsArrayList, 39. equalsRange, 
40. checkForComodification, 41. hashCodeRange, 42. outOfBoundsMsg, 43. outOfBoundsMsg, 44. shiftTailOverGap, 45. batchRemove, 46. elementAt, 47. removeIf, 48. removeIf, 49. nBits, 
50. setBit, 51. isClear, 52. replaceAllRange, 53. getFirst, 54. getLast, 55. addFirst, 56. addLast, 57. removeFirst, 58. removeLast, 59. removeRange, 
60. removeAll, 61. retainAll, 62. listIterator, 63. listIterator, 64. checkInvariants, 
```

# ✅ Javascript Program to Print All Array Methods:
```javascript
const arrayMethods = Object.getOwnPropertyNames(Array.prototype)
  .filter(prop => typeof Array.prototype[prop] === 'function');
console.log(arrayMethods);
```
## Output
```bash
[
  'constructor',    'at',        'concat',
  'copyWithin',     'fill',      'find',
  'findIndex',      'findLast',  'findLastIndex',
  'lastIndexOf',    'pop',       'push',
  'reverse',        'shift',     'unshift',
  'slice',          'sort',      'splice',
  'includes',       'indexOf',   'join',
  'keys',           'entries',   'values',
  'forEach',        'filter',    'flat',
  'flatMap',        'map',       'every',
  'some',           'reduce',    'reduceRight',
  'toLocaleString', 'toString',  'toReversed',
  'toSorted',       'toSpliced', 'with'
]
```
# ✅ Python Program to Print All Array Methods:
```python
import array
# Create a sample array
arr = array.array('i', [1, 2, 3])
# Print all available methods and attributes
print(dir(arr))
```
# Output
```bash
['__add__', '__buffer__', '__class__', '__class_getitem__', '__contains__', '__copy__', '__deepcopy__', '__delattr__', '__delitem__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getstate__', '__gt__', '__hash__', '__iadd__', '__imul__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__module__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__release_buffer__', '__repr__', '__rmul__', '__setattr__', '__setitem__', '__sizeof__', '__str__', '__subclasshook__', 'append', 'buffer_info', 'byteswap', 'count', 'extend', 'frombytes', 'fromfile', 'fromlist', 'fromunicode', 'index', 'insert', 'itemsize', 'pop', 'remove', 'reverse', 'tobytes', 'tofile', 'tolist', 'tounicode', 'typecode']
```
