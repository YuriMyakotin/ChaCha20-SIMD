# ChaCha20-SIMD

Chacha20 SIMD - SSE2, AVX2, AVX512 - C implementation (will add Arm64 implementation later).

SSE2 and AVX2 implementations based on code from Cryptopp. Avx512 code - made by myself (adapted avx2 version).

Some little benchmarking (Ryzen 9 7950X):
Avx512:
Encrypting 65536 bytes x 1000000 times: 9350.129 ms
255 bytes x 1000000 times: 90.367ms
64 bytes x 1000000 times : 77.506ms

Avx2:
17026.156 ms
142.672ms
68.288ms

Sse2:
32344.930 ms
276.484ms
67.759ms


Portable version (non-simd):
135420.469 ms
555.392ms
133.622ms



