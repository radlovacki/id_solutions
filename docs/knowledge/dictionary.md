# Акроними

## A

* **ACL** - Access Control List. A set of permissions stored in the tag’s
memory sectors (trailer block with keys and access bits).
* **ACL** - Allocation Class. Fixed 8-bit value in MSB of block 1 page 1 that
helps categorize the organization responsible for allocating UIDs to the tags.
`E0h` is the value for ATA5577.
[ISO/IEC 15963-1](https://www.iso.org/standard/73195.html).
* **AFE** - Analog Front End. All circuits that are directly connected to the
coil terminals in the transponder.
* **AFI** - Application Family Indicator. Memory block in the upper part of the
tag's memory that identifies the tag's application area. Some manufacturers use
the AFI code for security purposes.
* **Anti-Collision** - Technology that prevents multiple tags from interfering
with each other when they are read simultaneously.
* **ATA5577** (**ATA5577C**, **T5577**). R/W IC found in LF tags - can emulate
other LF formats.
* **ATQA** - Answer To Request (acc. to ISO/IEC 14443-4)
* **ATS** - Answer To Select (acc. to ISO/IEC 14443-4)
* **AWID** - Applied Wireless Identification Group. Manufacturer of RFID
products such as proximity cards, key fobs, vehicle tags and readers.

## B

* **Bi-phase** - modulation. A method used by the transponder (tag) to send
data back to the reader.

## C

* **CID** - Chip ID. 5-bit field, specifically bits 17 to 21 in block 1 page 1,
used to distinguish between different variations or specific models within the
broader ATA5577 family of integrated circuits (`00001b` for ATA5577M1, `00010b`
for ATA5577M2).
* **CL** - Cascade Level (acc. to ISO/IEC 14443-3)
* **COS** - Card Operating System
* **Cotag**. Dual-technology LF tags, that combine active (battery-powered) and
passive technology.
* **CRC** - Cyclic Redundancy Check. Error-detection method that generates a
short, fixed-length value called a checksum to verify the integrity of digital
data.
* **CT** - Cascade Tag, Type A
* **CUID** - Changeable Unique Identifier. Special type of identifier used on
certain tags, where the normally fixed UID can be modified.

## D

* **DIF** - Dual Interface (cards)

## E

* **EM4100**
* **EM410x**
* **EM4x05**
* **EEPROM** - Electrically Erasable Programmable Read-Only Memory. Type of
non-volatile memory that retains data even when power is turned off

## F

* **FDX-B**
* **FlexPass**
* **FSK** - Frequency Shift Keying - modulation. A method used by the
transponder (tag) to send data back to the reader.

## G

## H

* **HF** - High Frequency

## I

* **ICR** - IC Revision. 3-bit field, specifically bits 22 to 24 in block 1
page 1, used for the IC and/or foundry version of the ATA5577.
* **IDIC** - Identification Integrated Chip (Identification Integrated
Circuit). Specific types of integrated circuits used in RFID applications,
primarily operating in the LF range.

## J

## K

## L

* **LF** - Low Frequency

## M

* **Manchester** - modulation. A method used by the transponder (tag) to send
data back to the reader.
* **MFC** - Manufacturer Code. Second byte of block 1 page 1. Value `15h` is
for Atmel/Microchip. [ISO/IEC 7816-6](https://www.iso.org/standard/77181.html).
* **MSB** - Most Significant Byte. The byte in a multi-byte number that has the
greatest weighted value or influence on the total value of that number.

## N

* **NDEF** - NFC Data Exchange Format
* **NFC** - Near Field Communication
* **NRZ** - Non-Return-to-Zero - modulation. A method used by the transponder
(tag) to send data back to the reader.
* **NUID** -  Non-Unique Identifier. Tag identifier that is not guaranteed to
be globally unique.

## O

## P

* **PCD** - Proximity Coupling Device (“Contactless Reader”)
* **PICC** - Proximity Integrated Circuit (“Contactless Card”)
* **PKE** - Public Key Encryption (like RSA or ECC)
* **Proximity tag** (**proximity card**, **prox card**, **key card**,
**keycard**). Original 125 kHz tag without a smart chip, that doesn't hold more
data than a magnetic stripe card.
* **PSK** - Phase Shift Keying - modulation. A method used by the transponder
(tag) to send data back to the reader.

## Q

## R

* **REQA** - Request Command, Type A
* **RFID** - Radio Frequency Identification
* **RFU** - Reserved for future use
* **RID** - Random ID, typically dynamically generated at Power-on Reset (UID0
= “0x08”, Random number in UID1… UID3)

## S

* **SAK** - Select Acknowledge, Type A
* **Select** - Select Command, Type A

## T

* **T55xx**

## U

* **UHF** - Ultra High Frequency
* **UID** - Unique Identifier, Type A. A unique number assigned to each RFID
tag by the manufacturer.

## V

* **Vicinity tag** (**Vicinity card**, **VICC**). Contactless HF RFID tags
designed for longer reading ranges compared to proximity tags. Based on
[ISO/IEC 15693](https://www.iso.org/standard/70837.html) standard developed by
[ISO/IEC JTC 1/SC 17](https://www.iso.org/committee/45144.html) committee.

## W

## X

## Y

## Z
