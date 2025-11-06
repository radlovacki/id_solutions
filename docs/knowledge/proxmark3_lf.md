# Клонирање LF тагова

## Читање оригиналног тага

```text hl_lines="1 7"
[usb] pm3 --> lf search

[=] Note: False Positives ARE possible
[=]
[=] Checking for known tags...
[=]
[+] EM 410x ID 280074DE40
[+] EM410x ( RF/64 )
[=] -------- Possible de-scramble patterns ---------
[+] Unique TAG ID      : 14002E7B02
[=] HoneyWell IdentKey
[+]     DEZ 8          : 07659072
[+]     DEZ 10         : 0007659072
[+]     DEZ 5.5        : 00116.56896
[+]     DEZ 3.5A       : 040.56896
[+]     DEZ 3.5B       : 000.56896
[+]     DEZ 3.5C       : 116.56896
[+]     DEZ 14/IK2     : 00171806350912
[+]     DEZ 15/IK3     : 000085902392066
[+]     DEZ 20/ZK      : 01040000021407110002
[=]
[+] Other              : 56896_116_07659072
[+] Pattern Paxton     : 680074304 [0x28891C40]
[+] Pattern 1          : 13754820 [0xD1E1C4]
[+] Pattern Sebury     : 56896 116 7659072  [0xDE40 0x74 0x74DE40]
[+] VD / ID            : 040 / 0007659072
[+] Pattern ELECTRA    : 10240 7659072
[=] ------------------------------------------------

[+] Valid EM410x ID found!

[=] Couldn't identify a chipset
```

## Писање T5577 тагa

```text hl_lines="1"
[usb] pm3 --> lf em 410x clone --id 280074DE40
[+] Preparing to clone EM4102 to T55x7 tag with EM Tag ID 280074DE40 (RF/64)
[=] Encoded to FF 96 20 03 D3 BE A4 1C
[#] Clock rate: 64
[#] Tag T55x7 written with 0xff962003d3bea41c
[+] Done!
[?] Hint: Try `lf em 410x reader` to verify
```

## Провера

Оригинал:

```text hl_lines="1"
[usb] pm3 --> lf em 410x reader
[+] EM 410x ID 280074DE40
```

Копија:

```text hl_lines="1"
[usb] pm3 --> lf em 410x reader
[+] EM 410x ID 280074DE40
```
