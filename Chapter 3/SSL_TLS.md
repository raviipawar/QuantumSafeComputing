**Topics to be covered**

1. PKI (Public key infrastructure)
2. Encryption, Hashing, Digital Signatures
3. Installing and configuring PKI solutions
4. Secure socket layers (SSL)
5. Transport layer security (TLS)


1. PKI (Public key infrastructure)

    It is a collection/ hierarchy of digital security certificates.
    Certificates always contains public key. 
    Certificates can contain private keys too.
    Private keys can also be stored in seperate file.

    **PKI Components**

    1. Certificate Authority : issues, renews, revoke certificate. it also maintains CRL (certificate replication list, list of sno or revoked certs)

    2. Registration Authority : Also called a subordinate CA, should be used to manage CA 

    3. Certificate Revocation List (CRL) or Online certificate status protocol (OCSP) : Verification of certificate validity using a serial number.

    4. Certificate Template : Buleprint used when issuing certificate

    5. Certificate : It contains subject name, signature of CA, expiry information, public/private key.


    **Types of PKI Hierarchy**

    1. Single-Tier PKI Hierarchy (CA issues)
    2. Multi-Tier PKI Hierarchy  (CA -> RA -> issues certs)

    **Chain of Trust**

    1. CAs must be trusted authorities, otherwise PKI is meaningless
    2. Certificates contians the digital signature of issuing CA
    3. Digital signatures that are created with a private key are not easily spoofed
    4. Digital signatures are verified using the related public key
    5. Self-signed CAs can be used within an organization
    5. Nothig will trust a self signed CA by default
    6. CA certificates can be added to device trusted certificate store to supress warning messages.


    **PKI Certificates**

    1. Also called as X.509 certificates
    2. issued to users, devices, applications 
    3. have specific uses such as file encyprtion, securing network traffic using SSL, code signingl defined in certificate template
    4. Canbe stored in files on devices, on smart cards in firware (TPM)

    **PKI certificates contains**

    1. Version number
    2. Serial number
    3. CA digital signature and algorithm used
    4. Validity period
    5. Certifcate usage details
    6. Subject name, URL , email address
    7. Public/Private key 

    **SSL vs TLS**

    These both are the protocols to secure network communications.

    1. Both uses PKI
    2. Allows Encryption
    3. Allows Digital Signature and hashing (authentication, integrity, non-repudiation)
    4. Application Specific ( it must me sperately configured for HTTP, SMTP,,)

    **SSL**

    Developed by Netscape in early 1990.
    SSL v1-v3 none of these should be used uless required for leagcy interoperability.
    Superseded by TLS.
    SSL has security vulnerabilities so it should be disabled on servers.

    **Security Porotocol Downgrade attack**
    Disable SSL, enable TLS 1.1. or better

    **POODLE Attack**
    padding oracle on downgraded legacy encrytion.
    Affects SSLv3
    Malicious Javascript is injected into victims web browser using SSL v3 instead of TLS.
    Secure HTTP session cookies could be compromised.

    **Heartbleed Bug**

    **TLS**

    Transport Security Layer
    Replaces SSL
    TVS v1.0-1.3 
    Disable TLS v1.0 this is required to complywith PCI DSS 