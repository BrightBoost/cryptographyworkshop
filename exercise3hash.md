# **Hash Comparison Lab: “Same Length, Totally Different”**

### *A mini-workshop to understand hashing, fixed-length output, and tiny changes*

---

# 1. **What Is a Hash? (Short Explanation)**

A hash function takes input data and turns it into a fixed-length string.

The input can be short:

```
hello
```

Or very long:

```
a full document, image, video, or software file
```

But the hash output has a fixed length for that specific algorithm.

For example:

* MD5 always produces the same output length
* SHA-1 always produces the same output length
* SHA-256 always produces the same output length

A hash is like a fingerprint of the input.

> Important: a hash is not encryption.
> You cannot decrypt a hash back into the original data.

---

# 2. **Generate Your First Hash**

Use an online hash generator, for example:

https://emn178.github.io/online-tools/sha256.html

Or use another hash generator your trainer provides.

Hash this word using **SHA-256**:

```
hello
```

Write the SHA-256 hash here:

```
SHA-256 hash: ________________________________________________
______________________________________________________________
```

Now answer:

```
How many characters does the hash have? ______________________
```

---

# 3. **Tiny Change, Big Difference**

Now hash these three inputs using **SHA-256**.

Be careful: they look similar, but they are not the same.

### Input A

```
hello
```

Hash:

```
______________________________________________________________
______________________________________________________________
```

### Input B

```
Hello
```

Hash:

```
______________________________________________________________
______________________________________________________________
```

### Input C

```
hello 
```

There is a space after `hello`.

Hash:

```
______________________________________________________________
______________________________________________________________
```

Now compare the results.

Questions:

1. Are the hashes the same or different?

```
______________________________________________________________
```

2. What changed between input A and input B?

```
______________________________________________________________
```

3. What changed between input A and input C?

```
______________________________________________________________
```

4. Did a tiny change create a very different hash?

```
______________________________________________________________
```

---

# 4. **Same Input, Same Hash**

Hash this input twice using **SHA-256**:

```
cryptography is fun
```

### First result

```
______________________________________________________________
______________________________________________________________
```

### Second result

```
______________________________________________________________
______________________________________________________________
```

Now answer:

```
Are the two hashes the same? _________________________________
```

Reflection:

```
What does this tell you about hashing the exact same input twice?

______________________________________________________________
______________________________________________________________
```

---

# 5. **Different Algorithms, Different Lengths**

Hash this same input using **MD5**, **SHA-1**, and **SHA-256**:

```
it is friday
```

### MD5

```
Hash: ________________________________________________________
Length: ______________________________________________________
```

### SHA-1

```
Hash: ________________________________________________________
Length: ______________________________________________________
```

### SHA-256

```
Hash: ________________________________________________________
Length: ______________________________________________________
```

Now answer:

1. Which algorithm produced the shortest hash?

```
______________________________________________________________
```

2. Which algorithm produced the longest hash?

```
______________________________________________________________
```

3. Did the input stay the same each time?

```
______________________________________________________________
```

4. Why did the output length change?

```
______________________________________________________________
______________________________________________________________
```

---

# 6. **Hashing a Sentence**

Hash the following sentence using **SHA-256**:

```
Hashing protects integrity.
```

Hash:

```
______________________________________________________________
______________________________________________________________
```

Now change the period `.` into an exclamation mark `!`

```
Hashing protects integrity!
```

Hash:

```
______________________________________________________________
______________________________________________________________
```

Questions:

1. Did the sentence change a lot or only a little?

```
______________________________________________________________
```

2. Did the hash change a lot or only a little?

```
______________________________________________________________
```

3. Why is this useful for checking whether a file or message has changed?

```
______________________________________________________________
______________________________________________________________
```

---

# 7. **Can You Reverse a Hash?**

Look at this SHA-256 hash:

```
2cf24dba5fb0a30e26e83b2ac5b9e29e1b161e5c1fa7425e73043362938b9824
```

Try to answer without using a reverse lookup website.

Questions:

1. Can you decrypt this hash?

```
______________________________________________________________
```

2. Is hashing the same as encryption?

```
______________________________________________________________
```

3. What is the main purpose of hashing?

```
______________________________________________________________
______________________________________________________________
```

---

# 8. **Hashing for File Integrity**

Imagine you download a software installer.

The website says the correct SHA-256 hash should be:

```
abc123...
```

After downloading the file, your computer calculates:

```
abc123...
```

Question:

```
Does this suggest the file is unchanged? ______________________
```

Now imagine your computer calculates:

```
9f8e7d...
```

Question:

```
Does this suggest the file may have changed? _________________
```

Explain briefly:

```
______________________________________________________________
______________________________________________________________
```

---

# 9. **Reflection Question**

Write one or two sentences.

Why is hashing useful in cryptography?

```
______________________________________________________________
______________________________________________________________
______________________________________________________________
```

---

# **Bonus Challenge: Make a Hash Puzzle**

Pick a short secret word.

Hash it using **SHA-256**.

Write only the hash here:

```
My hash: _____________________________________________________
______________________________________________________________
```

Exchange with a classmate.

They may try to guess your original word.

Questions:

1. Was it easy to guess the original word?

```
______________________________________________________________
```

2. Would it be easier if the word was common, like `cat`, `admin`, or `password`?

```
______________________________________________________________
```

3. What does this teach us about hashing passwords?

```
______________________________________________________________
______________________________________________________________
```

---
