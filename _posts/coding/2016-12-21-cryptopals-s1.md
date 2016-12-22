---
layout: post
title: Cryptopals Set 1
category: coding
tags: python, cryptopals
comments: true
share: true
---

I learnt python few years ago with <a href="https://learnpythonthehardway.org/">"Learn Python the hard way"</a> and was pleasently surprised how compact code was while solving problems on <a href="https://projecteuler.net/"> Euler Project.

Fast-forward a few years, I wanted to brush up on the language and found out about <a href="https://cryptopals.com"> Cryptopals</a>. I had tried the cryptology MOOC on Udacity before but it was very theoretical and dry. This was much more practical and fun. It took a week to get through the first set because of all the 'gotchas' hurdles on the way. This series will be highlighting the stumbling blocks I faced rather than explaining solutions, you can figure that out by the vast number of gits already online

<a href="https://github.com/nukeu666/cryptopals">My Solutions</a>

# Problem 1
I didn't know about python libraries and coded the base64 to hex converter manually. Learn your libraries, use them!

Another constant pain in the code is forcing padding and stripping prefixes. A decimal 1 will be converted to 0x1, now you have to strip the 0x and pad it to 2 characters. Be wary.

# Problem 2
Another problem where you will need to strip and pad accurately. Make a version that inputs a pair of strings since that will be more useful later on.

# Problem 3
Not only will you need to count letter frequency/probability, you can't forget the spaces. Spaces are an important part of language.

Letter frequencies can be stripped from wikipedia or copy them from here

```python
    LetterProbs=['.082','.015','.028','.043','.127','.022','.020','.061','.070','.002','.008','.040','.024','.067','.075','.019','.001','.060','.063','.091','.028','.010','.024','.002','.020','.001']
```
# Problem 4
YOu get to test problem 3 here, fairly strightforward if p3 works.

# Problem 5
Easy if you implemented p2 correctly. The catch is the input is a single string with a newline!

# Problem 6
First get your hamming method right. If the keylength is n, you should test with longer strings a multiple of n(like 10*n), using cipherlengths of n will not work, think about why.

# Problem 7
Finally get to play with the AES package, straightforward problem

# Problem 8
Readup about block ciphers and ECB then find keylength repeating strings