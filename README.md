# Leetcode
Summary of leetcode problems

#146 LRU Cache    ***hard

Python helped to implement this problem by using OrderedDict() function which is from collections

1.move_to_end(key, last=True)
Move an existing key to either end of an ordered dictionary. The item is moved to the right end if last is true (the default) or to the beginning if last is false. Raises KeyError if the key does not exist:
Example:
>>> d = OrderedDict.fromkeys('abcde')
>>> d.move_to_end('b')
>>> ''.join(d.keys())
'acdeb'
>>> d.move_to_end('b', last=False)
>>> ''.join(d.keys())
'bacde'

2.popitem(last=True)
The popitem() method for ordered dictionaries returns and removes a (key, value) pair. The pairs are returned in LIFO order if last is true or FIFO order if false.
Example:
>>> d = OrderedDict.fromkeys('abcde')
>>> d.popitem()
('e', None)
>>> ''.join(d.keys())
'abcd'
>>> d.popitem(last=False)
('a', None)
