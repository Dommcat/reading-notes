# 401 Class 18 Reading Notes

## Summary: This class is about Cryptography

**Qp**: What is the basic principle behind the Caesar Cipher, and how was it used historically?

**A**:The Caesar Cipher is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is shifted a certain number of places down the alphabet. For example, with a shift of 3, A would be replaced by D, B would become E, C would become F, and so on.

The Caesar Cipher works by choosing a shift value, which represents the number of positions down the alphabet each letter should be shifted. The shift value is kept secret by the sender and recipient of the message. To encrypt a message, each letter in the plaintext is shifted by the shift value. For example, if the shift value is 3 and the plaintext is "HELLO", each letter is shifted by 3 positions down the alphabet to produce the ciphertext "KHOOR".

To decrypt the message, the recipient simply needs to know the shift value and apply it in reverse to the ciphertext. In the case of the shift value of 3, the recipient would shift each letter in the ciphertext 3 positions up the alphabet to get the original plaintext.

Although the Caesar Cipher is a very basic encryption technique and can be easily broken, it provided an effective way to communicate secretly in its time.


**Qp**:What are the key differences between symmetric and asymmetric encryption? How is asymmetric used in secure communication today?

**A**:Symmetric encryption uses one secret key for both encryption and decryption, while asymmetric encryption uses two mathematically related keys - a public key for encryption and a private key for decryption. Asymmetric encryption is slower but more secure than symmetric encryption. Asymmetric encryption is used in secure web browsing (HTTPS) and email (PGP) to protect sensitive information from eavesdroppers.

**Qp**:How do computers generate random numbers, and what are the differences between true random number generation (TRNG) and pseudo-random number generation (PRNG)? Discuss their use cases in cryptography.

**A**:Computers generate random numbers using various methods, but most of them are deterministic processes that use mathematical algorithms or hardware generators. These methods generate numbers that appear random but are actually predictable and follow a certain pattern or formula.

Pseudo-random number generators (PRNGs) use mathematical algorithms to generate random numbers that are statistically random but can be reproduced if the seed value used to start the algorithm is known. A seed value is an initial value used to start the algorithm, and it determines the sequence of numbers that the algorithm generates. PRNGs are commonly used in cryptography because they can produce a long sequence of random numbers quickly and efficiently, which is necessary for many cryptographic applications.

True random number generators (TRNGs) use physical sources of randomness, such as atmospheric noise, thermal noise, or radioactive decay, to generate truly random numbers that are not predictable. TRNGs produce random numbers that are not based on any mathematical algorithm or formula, and they are considered to be the most secure method of generating random numbers. TRNGs are commonly used in cryptographic applications that require high levels of security, such as generating cryptographic keys.

In cryptography, the use of PRNGs and TRNGs depends on the level of security required for a particular application. For applications where a high level of security is required, such as generating cryptographic keys or creating secure communication channels, TRNGs are preferred because they produce truly random numbers that cannot be predicted. However, TRNGs can be slower and more resource-intensive than PRNGs, which are more efficient and suitable for applications that require less security, such as generating random numbers for simulation or games.

**Qp**:What’s the difference between encryption and decryption? Explain with an analogy.

**A**:Encryption and decryption are two processes used in cryptography to secure information. Encryption involves taking plain text, which is readable and understandable, and transforming it into a secret code using a specific algorithm and a key. Decryption, on the other hand, is the process of reversing encryption, where the secret code is converted back to plain text using the same algorithm and key.

An analogy for encryption and decryption is sending a secret message in a locked box. Imagine you have a message that you want to keep secret, so you put it inside a locked box. The box represents encryption, where the message is transformed into a secret code using a key (the lock) and an algorithm (the box). Only the person with the key can open the box and read the message, which represents decryption. If someone intercepts the box during transmission, they will not be able to read the message without the key to unlock the box.

In this analogy, encryption is like locking the box, and decryption is like unlocking the box. Without the key, the secret message inside the box is secure and cannot be read by anyone else. Similarly, encryption makes sure that data transmitted over the internet is secure and unreadable by anyone without the key, making it a crucial component in securing sensitive information.

**Prompt**:

Watch the video linked inside What is is Jupyter Lab reading

## Sources:

ChatGpt

https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html

https://www.dataquest.io/blog/numpy-tutorial-python/

https://www.tutorialspoint.com/numpy/index.htm

https://www.howtogeek.com/183051/htg-explains-how-computers-generate-random-numbers/

https://thebestvpn.com/cryptography/


## Things I want to know more about

Random Number Generators 