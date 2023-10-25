**Table of Contents**

1. Cryptography
2. Encryption
3. Secure Hashing
4. Digital Signatures
5. Public Key Infrastructure
6. Transport Layer Security
7. Mathematical concepts used in cryptographic algorithms
8. Understanding computational complexity of algorithms

**1. Cryptography**

        What is Cryptography ?

        Providing the security and protection to the data in rest or in motion.
        Cryptography lays the foundation of building the secure systems.
        There are various crypto algorithms and crypto libraries present which are used to secure system and data.


        What are the Main Pillars of Cryptography ?

        1. Authenticity
        2. Confidentiality
        3. Integrity
        4. Non Repudiation

        Authenticity    : It  validates the origin of the message/data
                          Users can validate where the data is coming from
                          Digital certificates help achieve this

        Confidentiality : It ensures that the message transmitted is only visible to users authorized to see it 
                          It must guarantee the secure transmission of data across insecure channels
                          Symmetric & asymmetric encryption helps achieve this
                              
        Data Integrity  : It deals with making sure that data is not tampered by unauthorized users 
                          It Must guarantee data remains intact during transmission
                          It can be achieved by using hashing

        Non-repudiation : It enables the users to guarantee the origin of the data in an undisputable manner    
                          It Must guarantee that data is from who it says it is from
                          Digital signatures can help achieve this


    **Cryptographic Terminology**

        1. Cryptographic protocols : They define the protocols, rules, syntax and semantics to perform a specific security related  operation
        2. Cryptographic Algorithms : (ciphers) It defines a set of instructions to perform a specific cryptographic functions
                    Examples : Digital Signature Algorithm to authenticate entities
                               Asymmetric/Symmetric algorithm for encryption/decryption
                               Hash function algorithm to ensure data integrity.
        3. Key Management : Cryptography algos may use keys to provide certain cryptographic functions
                            It Manages the generation, exchange, storage, use, replacement, and destruction of keys used in 
                            encryption/decryption
                            Example:  Encryption algorithms use keys to encrypt and decrypt data to ensure confidentiality
        

**Types of Cryptography**

1. Classical/Traditional Cryptography
     Based on principles of mathematics and relies on the computational difficulty of large number factorization and discrete 
     logarithms. 
     Designed for classical computers Difficult (but not impossible) to decrypt data that is encrypted using classical 
     cryptography by classical computers (can take thousands of years). With quantum computers data can be easily decrypted

2. Quantum Safe Cryptography
      Also based on the principles of mathematics, but the cryptographic algorithms are based on more complex math calculations that are resistant to quantum computers
      Designed for both classical and quantum computers
      
3. Quantum Cryptography
     Data is transmitted as qubits using particles of light called photons through optic fiber cables
     Based on principles of quantum/modern physics. Security of the system depends on the properties of quantum mechanics which relies on the following guarantees:
            • Heisenberg Uncertainty Principle - particles can exist in more than one place or state at a time
            • Photon Polarization Principle - qubits cannot be observed without changing or disturbing it, hence cannot be copied