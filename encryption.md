## Encryption
Encryption is the practice of scrambling information in a way that only someone with a corresponding key can unscramble and read it. Encryption is a two-way function. When you encrypt something, you’re doing so with the intention of decrypting it later. This is a key distinction between encryption and hashing.

#### Cipher
To encrypt data you use something called a cipher, which is an algorithm – a series of well-defined steps that can be followed procedurally – to encrypt and decrypt information

#### common forms of encryption are:

* Asymmetric Encryption – This is the Public Key example we just gave. One key encrypts, the other key decrypts. The encryption only goes one way. This is the concept that forms the foundation for PKI (public key infrastructure), which is the trust model that undergirds SSL/TLS. 
* Symmetric Encryption – This is closer to a form of private key encryption. Each party has its own key that can both encrypt and decrypt. As we discussed in the example above, after the asymmetric encryption that occurs in the SSL handshake, the browser and server communicate using the symmetric session key that is 


## Hashing
Hashing is the practice of using an algorithm to map data of any size to a fixed length. This is called a hash value (or sometimes hash code or hash sums). Whereas encryption is a two-way function, hashing is a one-way function. While it’s technically possible to reverse hash something, the computing power required makes it unfeasible. Hashing is one-way. Now, whereas encryption is meant to protect data in transit, hashing is meant to verify that a file or piece of data hasn’t been altered—that it is authentic.


## Salt
Salting is a concept that typically pertains to password hashing. Essentially, it’s a unique value that can be added to the end of the password to create a different hash value. This adds a layer of security to the hashing process, specifically against brute force attacks. A brute force attack is where a computer or botnet attempt every possible combination of letters and numbers until the password is found. Anyway, when salting, the additional value is referred to as a “salt.”

Say the password I want to salt looks like this: 7X57CKG72JVNSSS9 Your salt is just the word SALT Before hashing, you add SALT to the end of the data. So, it would look like this: 7X57CKG72JVNSSS9SALT

Read more at: https://www.thesslstore.com/blog/difference-encryption-hashing-salting/
