# **XOR Cipher Exercise: “The Magical Reversible Operation”**

### _A mini-workshop to understand XOR and why cryptographers love it_

---

# 1. **What Is XOR? (Short Explanation)**

XOR is a tiny logical operation used in almost all modern cryptographic algorithms.

The rule is simple:

> **If two bits are different → XOR = 1
> If they are the same → XOR = 0**

Here’s the full truth table:

| A   | B   | A XOR B |
| --- | --- | ------- |
| 0   | 0   | 0       |
| 0   | 1   | 1       |
| 1   | 0   | 1       |
| 1   | 1   | 0       |

You’ll use this rule for all exercises.

---

# 2. **Warm-up: XOR These Bits**

Compute the XOR of each pair:

a) `1 XOR 0 = ______`
b) `0 XOR 0 = ______`
c) `1 XOR 1 = ______`
d) `0 XOR 1 = ______`
e) `1 XOR 0 XOR 1 = ______`

(_If stuck, check the truth table above._)

---

# 3. **XOR a Whole Byte (Bit by Bit)**

Use the XOR rule for each pair of bits.

Plaintext byte:

```
P = 01011010
```

Key byte:

```
K = 11100010
```

Task: compute

```
C = P XOR K
```

Write your result here (8 bits):

```
C = __________________________________
```

---

# 4. **Show That XOR Is Reversible**

Now decrypt the ciphertext by XORing it with the same key:

We already have:

```
C = P XOR K
```

To recover P:

```
P = C XOR K
```

Perform the XOR again (bit by bit):

```
P = __________________________________
```

**You should get the original P again.**

> This shows why XOR is magical:
> **XORing twice with the same key undoes itself.**

---

# 5. **Encrypt and Decrypt a Short Message Using XOR**

We’ll use a tiny symmetric cipher:

- Convert letters to decimal ASCII
- XOR with a small key
- Convert back to letters

### Step A — Convert letters to ASCII

Message:

```
FUN
```

ASCII codes:
F = **_
U = _**
N = \_\_\_

(_Hint: use an online ASCII table: [https://www.asciitable.com/](https://www.asciitable.com/)_)

---

### Step B — XOR with key = **7**

Compute:

```
Cipher = ASCII_value XOR 7
```

F → **\_\_**
U → **\_\_**
N → **\_\_**

(_This gives you three numbers: the ciphertext._)

---

### Step C — Decrypt

Now decrypt by XORing the ciphertext numbers with the same key:

```
Plain = Cipher XOR 7
```

You should get back the ASCII codes for **F U N**.

Write your results:

F → **\_\_**
U → **\_\_**
N → **\_\_**

---

# 6. **Apply XOR Encryption to “it is friday”**

We’ll encrypt letters one by one, using key = **3**
(You can remove spaces or keep them as ASCII 32.)

Pick three letters from the phrase (e.g., `i`, `t`, space).

For each letter:

1. Look up ASCII
2. XOR with 3
3. Write ciphertext
4. Decrypt again to confirm reversibility

### Example Template:

Letter: **\_**
ASCII: **\_**
Cipher = ASCII XOR 3 = **\_**
Decrypt = Cipher XOR 3 = **\_**

Do this for 3 different characters.

---

# 7. **Reflection Question (Write in One Sentence)**

Why do you think XOR is useful in encryption, especially in stream ciphers?

Answer:

```
__________________________________________________________
__________________________________________________________
```

---
