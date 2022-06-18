This repository contains simple benchmarks of various Rust serialization
libraries.

# Running

On Rust nightly run `cargo bench`.

# Results

```
test deserialize_manual                       ... bench:          49 ns/iter (+/- 26)
test deserialize_manual_foreign_endianness    ... bench:          53 ns/iter (+/- 27)
test deserialize_serde_bincode                ... bench:         104 ns/iter (+/- 10)
test deserialize_speedy                       ... bench:          66 ns/iter (+/- 11)
test deserialize_speedy_foreign_endianness    ... bench:          65 ns/iter (+/- 11)
test deserialize_speedy_foreign_endianness_ne ... bench:          72 ns/iter (+/- 13)
test deserialize_speedy_ne                    ... bench:          72 ns/iter (+/- 4)
test serialize_manual                         ... bench:          28 ns/iter (+/- 3)
test serialize_manual_foreign_endianness      ... bench:          29 ns/iter (+/- 11)
test serialize_prost                          ... bench:          54 ns/iter (+/- 1)
test serialize_rmp                            ... bench:          68 ns/iter (+/- 8)
test serialize_serde_bincode                  ... bench:          75 ns/iter (+/- 5)
test serialize_serde_cbor                     ... bench:         224 ns/iter (+/- 5)
test serialize_serde_json                     ... bench:         403 ns/iter (+/- 142)
test serialize_serde_pickle                   ... bench:         194 ns/iter (+/- 4)
test serialize_serde_rmp                      ... bench:         178 ns/iter (+/- 12)
test serialize_serde_xdr                      ... bench:          79 ns/iter (+/- 3)
test serialize_speedy                         ... bench:          48 ns/iter (+/- 3)
test serialize_speedy_foreign_endianness      ... bench:          48 ns/iter (+/- 0)
test serialize_speedy_foreign_endianness_ne   ... bench:          52 ns/iter (+/- 3)
test serialize_speedy_ne                      ... bench:          51 ns/iter (+/- 0)
```
