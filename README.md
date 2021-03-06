# Word Frequency Counter

## Description

Developed for an Operating Systems course; gain experience with threads and processes developing a simple command line app to count the number of repeated words in a text file.

## Use

``` C
git clone https://github.com/skylerto/count-words.git

cd count-words

make
./count //{filename(s)}    // Single thread
./process //{filename(s)}  // Multi process
./thread //{filename(s)}   // Multi thread
```

## Examples

Ran on...  
![alt tag](/img/specs.png)

#### Single Threaded
```
count-words $ time ./count dataset*
dataset1.txt: 561 OK AND A
dataset2.txt: 600 A AND IT'S
dataset3.txt: 574 A IT'S OK

real	0m2.152s
user	0m2.035s
sys	0m0.019s
```

#### Multi Process
```
count-words $ time ./process dataset*
dataset2.txt: 600 A AND IT'S
dataset3.txt: 574 A IT'S OK
dataset1.txt: 561 OK AND A

real	0m0.928s
user	0m1.431s
sys	0m0.012s
```

#### Multi threaded
```
count-words $ time ./thread dataset*
dataset2.txt: 600 A AND IT'S
dataset3.txt: 574 A IT'S OK
dataset1.txt: 561 OK AND A

real	0m0.897s
user	0m2.298s
sys	0m0.016s
```

## License

The MIT License (MIT)

Copyright (c) 2015 Skyler Layne

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
