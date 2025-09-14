All intelligence is basically compression. Not exactly, but pretty close.

What is compression? -> Representing information in a smaller manner, without losing any quality.

Compression and prediction come close to each other too.

Prediction is a pretty clear sign of intelligence.
For example, a sequence of numbers:
```
2222
```

Can be represented as:
```
4*2
```

Option 2 is compressed, and if I wanted to predict the next number in the sequence, given the compressed version, I have:
```
5*2
```

Thing is though, I have to know how to de-compress the compressed version. If I were to write a program in python to do it, it would look something like:
```python
def main(compressed_value: str) -> str:
    number_of_items, value = compressed_value.split("*")
    decompressed_value = []
    for i in range(number_of_items):
        decompressed_value.append(value)

    return decompressed_value.join(",")
```

This decompression program has to be packed together with the compressed version and together they're sort of complete.

This is not the perfect example of compression especially when dealing with small number of values cause the size of the decompression program is much larger than actual value of items. But when the number of repetitions becomes larger say ```1000*2```, then it's okay.

This is the idea behind the [Hutter Prize](http://prize.hutter1.net/). And I have to say it's not a bad place to start.

If you have 2 sets of programs for compressing and decompressing information and one of them results in a smaller compressed output, and both of them result in the exact & correct output, and given that both of them run on the same compute, then the smaller one can be said to be more intelligent. It can be said to understand better.

A human brain for example is an extremely efficient way of compressing memories, sensory inputs etc. and a very efficient decompression program that enables us to act/(predict what to do next).

This is very interesting cause if you can predict things perfectly and you are never wrong, then you are the most intelligent person. For example, last year at the attempted Trump assasination, if you saw that then you thought that he would win the election because of the emotions that stirred and as a result of him winning the elections the U.S government would lean more into crypto and the price of bitcoin would go up. If you were able to predict that, dude...

It wouldn't even matter if that was the exact reasoning that made the outcome, if you could somehow use the experience of the world that you have and come up with a true prediction, then no one can stand against you. You would have to reproduce this a couple of times before we elect you ruler of the world of course 😂. But if you did, dude...
