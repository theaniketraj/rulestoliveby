# Kerckhoffs's Principle

> "A cryptosystem should be secure even if everything about the system, except the key, is public knowledge."

**The Insight:**  
Security through obscurity is valid only as a temporary delay measure, not as a defense. If your security depends on nobody guessing your algorithm, you are already hacked.

**In Practice:**  
Assume the attacker has your source code. Assume they have your database schema. The only thing they shouldn't have is the private keys/passwords. Use standard, open-source crypto libraries (AES, RSA, bcrypt) that have been battle-tested by the world, rather than inventing your own "secret" encryption.
