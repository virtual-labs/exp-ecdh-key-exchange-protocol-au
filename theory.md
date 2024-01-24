# Elliptic-curve Diffie–Hellman (ECDH) Key Exchange Protocol
The Elliptic-curve Diffie–Hellman (ECDH) Key Exchange Protocol is a cryptographic algorithm used to establish a shared secret key between two parties over an insecure communication channel. This process ensures secure communication by allowing the parties to derive a common secret without transmitting it directly.

## User Key Generation
### User A's Key Generation
1. **Private Key Selection (User A):** The private key for User A (\(nA\)) is chosen, satisfying the condition \(nA < n\).
2. **Public Key Calculation (User A):** The corresponding public key (\(PA\)) is calculated using the formula \(PA = nA \times G\).

### User B's Key Generation
1. **Private Key Selection (User B):** Similarly, the private key for User B (\(nB\)) is chosen, ensuring \(nB < n\).
2. **Public Key Calculation (User B):** The public key (\(PB\)) for User B is computed as \(PB = nB \times G\).

## Secret Key Derivation
1. **Secret Key Calculation (User A):** The secret key (\(K\)) for User A is determined by multiplying their private key (\(nA\)) with User B's public key (\(PB\)): \(K = nA \times PB\).
   
2. **Secret Key Calculation (User B):** Similarly, the secret key (\(K\)) for User B is calculated by multiplying their private key (\(nB\)) with User A's public key (\(PA\)): \(K = nB \times PA\).

Both User A and User B now possess a shared secret key (\(K\)).
