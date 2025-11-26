# t55xx

## Memory map


``` text title="T5577 Memory Map"
          0   1  2  3  4  5  6  7  8  9  10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32
Page 1  ┌───┬────────────────────────────────────────────────────────────────────────────────────────────────┐
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 3: Analog front end option set-up
        │ 1 │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 2: Traceability data
        │ 1 │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 1: Traceability data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 0: Page 0 configuration data
        └───┴────────────────────────────────────────────────────────────────────────────────────────────────┘
Page 2  ┌───┬────────────────────────────────────────────────────────────────────────────────────────────────┐
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 7: User data or password
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 6: User data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 5: User data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 4: User data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 3: User data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 2: User data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 1: User data
        │ L │ 0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0  0 │ Block 0: Configuration data
        └───┴────────────────────────────────────────────────────────────────────────────────────────────────┘
```

* 363-bit EEPROM - 11 blocks of 33 bits.
* First bit of each block is a lock bit, responsible for write-protecting the
associated block:
    * `0` unlocked
    * `1` locked


Programming takes place on a block basis, so a complete block (including lock
bit) is programmed simultaneously with a single command. Block 0 of page 0
contains the mode/configuration data, which are not transmitted during
Regular-Read mode operations.
