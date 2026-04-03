Activity A5: Discover cryptographic implementation used online

## Objective
To identify cryptographic techniques used in online communication.

## Methodology
I accessed a secure website (https://www.google.com) and examined the connection security details using the browser. I also inspected the SSL/TLS certificate information.

## Findings

### 1. HTTPS and TLS Encryption
The website uses HTTPS, which relies on TLS (Transport Layer Security) to encrypt communication between client and server.

### 2. Digital Certificate
The website provides a digital certificate issued by a trusted Certificate Authority (CA), which verifies the identity of the server.

### 3. Public Key Cryptography
TLS uses asymmetric encryption (public/private keys) to establish a secure connection, followed by symmetric encryption for efficient data transfer.

## Analysis
The use of HTTPS ensures confidentiality, integrity, and authenticity of online communication. It protects users from eavesdropping and man-in-the-middle attacks.

## Evidence
- Screenshot of browser showing HTTPS lock icon
- Screenshot of certificate details

## Reflection
This activity helped me understand how cryptography is applied in everyday online browsing. It shows that secure communication is achieved through a combination of encryption and authentication mechanisms.
