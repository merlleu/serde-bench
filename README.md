This repository contains simple benchmarks of various Rust serialization
libraries.

# Running

On Rust nightly run `cargo bench`.

# Results

```
test deserialize_manual                       ... bench:          85 ns/iter (+/- 6)
test deserialize_manual_foreign_endianness    ... bench:          99 ns/iter (+/- 4)
test deserialize_serde_bincode                ... bench:         141 ns/iter (+/- 4)
test deserialize_speedy                       ... bench:         101 ns/iter (+/- 5)
test deserialize_speedy_foreign_endianness    ... bench:         100 ns/iter (+/- 2)
test deserialize_speedy_foreign_endianness_ne ... bench:         111 ns/iter (+/- 3)
test deserialize_speedy_ne                    ... bench:         109 ns/iter (+/- 3)
test serialize_manual                         ... bench:          52 ns/iter (+/- 1)
test serialize_manual_foreign_endianness      ... bench:          47 ns/iter (+/- 0)
test serialize_prost                          ... bench:          66 ns/iter (+/- 2)
test serialize_rmp                            ... bench:          85 ns/iter (+/- 11)
test serialize_serde_bincode                  ... bench:          54 ns/iter (+/- 1)
test serialize_serde_cbor                     ... bench:         120 ns/iter (+/- 10)
test serialize_serde_json                     ... bench:         269 ns/iter (+/- 20)
test serialize_serde_pickle                   ... bench:         106 ns/iter (+/- 4)
test serialize_serde_rmp                      ... bench:         133 ns/iter (+/- 2)
test serialize_serde_xdr                      ... bench:          74 ns/iter (+/- 1)
test serialize_speedy                         ... bench:          48 ns/iter (+/- 0)
test serialize_speedy_foreign_endianness      ... bench:          49 ns/iter (+/- 2)
test serialize_speedy_foreign_endianness_ne   ... bench:          58 ns/iter (+/- 0)
test serialize_speedy_ne                      ... bench:          59 ns/iter (+/- 1)
```
