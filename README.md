# ChaCha12-Blake3
This is an experimental idea for a custom AEAD (Authenticated Encryption with Associated Data) that combines ChaCha12 for encryption and BLAKE3 for hashing and message commitment.
I came across this design in a Rust crate. It’s pretty interesting because it has message commitment that some AEADs don't have.

## Why ChaCha12 + BLAKE3?
ChaCha12 is a faster, reduced round variant of ChaCha20 while still being secure (anything above 8 rounds is considered secure).

BLAKE3 is the fastest hash from rbx-crypto.

Not recommended for production use.
