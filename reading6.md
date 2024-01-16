# Reading 6
# Data File Encryption
## Why this topic matters?


1. You have been made responsible for the company’s file server. How would you preserve the three elements of the CIA triad?

    1. Confidentiality:

    - Implement access controls: Set up user permissions and access controls to ensure that only authorized individuals can access sensitive data.
    - Encryption: Use encryption protocols to protect data both in transit and at rest. This prevents unauthorized access even if someone gains physical access to the server or intercepts data during transmission.

    2. Integrity:

    - Data validation: Implement mechanisms to validate the integrity of data. This can include checksums, hashing, or digital signatures to ensure that data has not been tampered with.
    - Version control: Maintain versioning for files to track changes and ensure that modifications are authorized. Regularly back up data and verify the integrity of backups.

    3. Availability:

    - Redundancy: Implement redundant systems, such as mirrored servers or backups, to ensure availability in case of hardware failures or other issues.
    - Disaster recovery planning: Develop a comprehensive disaster recovery plan that includes backup strategies, offsite storage, and quick recovery procedures to minimize downtime.

2. Explain how hashing verifies data integrity using non-technical terms.


Hashing, in simple terms, is like turning a piece of information, such as a document or a file, into a unique "fingerprint" or "smoothie" through a special algorithm. This fingerprint, known as the hash, is a fixed size and is unique to the specific content. Even a small change in the original information results in a completely different hash. When you want to share or verify the integrity of the information, you provide others with this compact hash instead of the entire content. Recipients can use their own "blender" to generate a hash from the received information. If the hash they create matches the one you shared, it means the information hasn't been tampered with. It's like ensuring the recipe stays the same by exchanging and comparing magical smoothies.

3. How is hashing and encryption different?

    1. hashing

    - Purpose: Hashing is primarily used to verify data integrity. It transforms input data into a fixed-size string of characters, known as a hash value or hash code. The same input will always produce the same hash, but even a small change in the input will result in a significantly different hash. Hashing is a one-way process, meaning it cannot be reversed to obtain the original input.
    -  Key Feature: It is deterministic and designed for quick and efficient verification. Common hash functions include SHA-256 or MD5.


    2. Encryption:

    - Purpose: Encryption is used to protect data confidentiality. It transforms plaintext (original data) into ciphertext (unreadable data) using an algorithm and a key. The process is reversible, meaning the ciphertext can be decrypted back into the original plaintext if you have the key. Encryption is a two-way process designed to keep data secure during transmission or storage.
    - Key Feature: It involves the use of keys for both encryption and decryption. Common encryption algorithms include AES (Advanced Encryption Standard) and RSA.


    In summary, hashing is one-way and designed for data integrity verification, while encryption is a two-way process used to secure data by making it unreadable without the appropriate key. Hashing doesn't provide confidentiality, and encrypted data can be decrypted with the right key.

## Analogy

## Things I want to know more about:


## Sources:
- https://www.jscape.com/blog/implementing-the-cia-triad-when-transferring-files-through-the-internet
- https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/
- https://chat.openai.com/
