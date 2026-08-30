# Symmetric Encryption 
In symmetric Encryption same secret key is used for both Encryption and Decryption.
###### Message -> [Encryption (using secret key) ] -> Encrypted Message -> [Decryption (using same secret key) ] -> Message
#### Common symmetric algorithms
- AES --> Advanced Encryption Standard
- 3DES --> older and generally not preferred for new designs
#### Advantages
- Very fast
- Good for encrypting large amounts of data
# Asymmetric Encryption
Asymmetric Encryption uses two keys public and private keys. 
In Asymmetric Encryption public key uses for Encryption and private key uses for decryption. The private key must be remain secret.
###### Message -> [Encryption (Public key) ] -> Encrypted Message -> [Decryption (Private key) ] -> Message
#### Common algorithms
- RSA
- ECC (Elliptic Curve Cryptography)
- Diffie-Hellman
# Hashing
- A hash function converts input into a fixed-size output called a hash or digest.
- For a cryptographic hash, should not be able to practically reverse the hash to recover the original input.
### MD5
MD5(Message digest Algorithm 5) produces 128 bit(32 hexadecimal character) digest. It should not be used for security-sensitive integrity or password hashing.
### SHA-256
SHA-256(Secure Hash Algorithm-256) belongs to SHA-2 family. It produces 256 bit (64 hexadecimal character) digest.A tiny change in the input produces a completely different digest.
###### SHA-256 is used
- File integrity
- Digital signatures
- Certificates
- Software verification
# Digital Certificates
- A digital certificate helps establish that a public key belongs to a particular identity/domain.
- A digital certificate is basically an electronic identity document for a website/server
###### Website -> Public Key -> Digital Certificate -> Certificate Authority (CA)
- A Certificate Authority (CA) is a trusted organization that issues/signs certificates.
#### TLS/SSL
- SSL (Secure Sockets Layer) and TLS (Transport Layer Security) are cryptographic protocols.
- Designed to secure communication over the internet.  While SSL was the original protocol developed in the 1990s, it is now considered deprecated and insecure due to known vulnerabilities.  TLS is the modern secure successor that replaced SSL, offering stronger encryption, improved performance, and enhanced data integrity.
- If validation succeeds, the browser and server continue the TLS handshake and establish cryptographic keys for the connection.
  ###### TLS provides:
🔒 Confidentiality
🛡️ Integrity
✅ Authentication













