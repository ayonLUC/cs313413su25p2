Performance Results — SIZE = 1000, REPS = 100000

ArrayList Add/Remove: 71 ms
LinkedList Add/Remove: 82 ms
ArrayList Access: 34 ms
LinkedList Access: 28 ms

Conclusions:

- LinkedList is much faster for repeated add/remove at the front.
- ArrayList is much faster for index-based access.
- Choose based on use case: LinkedList for heavy insertions/deletions, ArrayList for fast reads.

---

Q: What happens if you use list.remove(Integer.valueOf(77)) inside a loop?
A: It removes the first match, but may cause ConcurrentModificationException if used while iterating.

Q: Behavioral difference between LinkedList and ArrayList?
A: None in correctness — just performance differences.

Q: What do list.remove(index) and list.remove(Object) do?
A: One removes by position, the other by value.
