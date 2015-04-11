# Caesar-Cipher-Python

Encryption is the process of obscuring information to make it unreadable without special knowledge.
A cipher is an algorithm for performing encryption (and the reverse, decryption). 
A cipher usually depends on a piece of auxiliary information, called a key. The key is incorporated into the encryption process; the same plaintext encrypted with two different keys should have two different ciphertexts. Without the key, it should be difficult to decrypt the resulting ciphertext into readable plaintext.

CAESAR CIPHER

The basic idea of the Caesar cipher is that you pick an integer for a key, and shift every letter of your message by the key. For example, if your message was "happy" and your key was 3, "h" becomes "k", "a" becomes "d", and so on, because we are shifting every letter three spots to the right. Here is what the whole alphabet looks like shifted three spots to the right:

 
Original:  a b c d e f g h i j k l m n o p q r s t u v w x y z
 3-shift:  d e f g h i j k l m n o p q r s t u v w x y z a b c
Using the above key, we can quickly translate the message "happy" to "kdssb" (note how the 3-shifted alphabet wraps around at the end, so x -> a, y -> b, and z -> c).

In this problem, we will use a variant of the standard Caesar cipher where we will treat upper and lower case letters separately, so upper case letters will always be mapped to upper case letters, and lower case letters will always be mapped to lower case letters. Thus, if "a" maps to "c", "A" will map to "C". Characters such as the space character, commas, periods, exclamation points, etc will not be encrypted by this cipher - basically, 

Decryption Of CAESAR CIPHER
If you know which shift key is used while encrypting, then decrypting message is an easy task.

The problem is, you don't know which shift key is used. So if you can write a program to find the decoding that produces the maximum number of real English words, you can probably find the right decoding
