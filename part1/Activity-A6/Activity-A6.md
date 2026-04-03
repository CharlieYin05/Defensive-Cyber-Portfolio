# Activity A6: Discover cryptographic implementation used offline

## Objective
To identify cryptographic techniques used in offline systems.

## Methodology
I examined the FileVault disk encryption feature on my MacBook Air. I reviewed both the system settings and official documentation describing how FileVault works.
![FileVault][screenshot/FileVailt.jpg]

## Findings

### 1. Full Disk Encryption
FileVault provides full disk encryption, protecting all data stored on the internal storage device.

### 2. Encryption Algorithm
FileVault uses AES-XTS encryption, which is a widely adopted standard for securing data at rest.


### 3. Key Management
The encryption system uses a hierarchy of cryptographic keys:
- Volume key (used to encrypt data)
- Key Encryption Key (KEK), protected by the user's password

### 4. Hardware Security Integration
On Apple silicon devices, encryption keys are managed by the Secure Enclave, ensuring that keys are not exposed to the main CPU.

### 5. Authentication Requirement
Access to encrypted data requires user authentication during boot. Without the correct password or recovery key, the data remains inaccessible.

## Analysis
FileVault ensures confidentiality of data even if the physical device is stolen. The use of AES-XTS encryption and hardware-backed key storage significantly enhances security.

The key hierarchy design also improves security by isolating encryption keys and allowing password changes without re-encrypting the entire disk.

## Evidence
- Screenshot showing FileVault enabled in system settings
- Screenshot of FileVault technical description (encryption and key hierarchy)

## Reflection
This activity demonstrated how cryptography is used in offline systems to protect data at rest. It highlights the importance of disk encryption and secure key management in modern computing devices.
