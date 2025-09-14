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

if __name__ == '__main__':
    main()
```

This decompression program has to be packed together with the compressed version and together they're sort of complete.

This is not the perfect example of compression especially when dealing with small number of values cause the size of the decompression program is much larger than actual value of items. But when the number of repetitions becomes larger say ```1000*2```, then it's okay.

This is the idea behind the [Hutter Prize](http://prize.hutter1.net/). And I have to say it's not a bad place to start.