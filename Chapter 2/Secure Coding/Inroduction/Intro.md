**Topics to be covered**

1. Secure against what link
2. Version control and security 
3. Secure coding practices
4. Storing data securely
5. The OWASP top 10

1. Encoding : Mapping of information to symbols 

2. Encryption : The process of converting the information into a secret form  which cannot be interpreted without knowing the secrey    method of encryption call the key.

    Crypto key Breakdown
        1. Public key 
            Sender   : Encrypt with recipient key 
            Reciever : Verify signed message with sender key
        
        2. Private key 
            Sender   : Sign message with own key 
            Reciever : Recipient decrypt using own key
    
    Hashing : Coverts the object/message to hash code
        
3. Serialization : The encoding of an object for storage or transport
                Format can be JSON, XML 
                Don't ever serialize to binary format 
                JSON is object notation 
                Don't confuse scopes with security

