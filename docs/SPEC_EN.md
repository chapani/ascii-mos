# ASCII-MOS: Technical Specification

This document defines the mapping rules for the ASCII-MOS (ASCII-compliant) standard to ensure 100% ASCII compatibility for Uzbek language identifiers.

## 1. Core Mapping Table


| Standard Uzbek | ASCII-MOS (Safe ASCII) | Rationale |
| :--- | :--- | :--- |
| **O‘ / o‘** | `oe` | Borrowed from the Germanic/Turkic convention for the closed 'O' sound (similar to `ö`). |
| **G‘ / g‘** | `gh` | Standard linguistic representation for the voiced velar fricative. |
| **’** (Glottal) | (Dropped) | Removed to keep identifiers short and avoid syntax errors. |


## 2. Capitalization Logic

To ensure compatibility with programming casing styles (PascalCase, camelCase):

1. **Lowercase:** `oʻzgarish` -> `oezgarish`, `gʻalvir` -> `ghalvir`
2. **Sentence/Title Case:** `Oʻzgarish` -> `Oezgarish`, `Gʻalvir` -> `Ghalvir`
3. **Uppercase:** `OʻZGARISH` -> `OEZGARISH`, `GʻALVIR` -> `GHALVIR`

## 3. Collision Resolution

The primary goal of ASCII-MOS is to maintain unique word roots.

**Standard Lossy Approach:**

* `bo‘sh` (empty) -> `bosh`
* `bosh` (head) -> `bosh`
* **Result:** Semantic collision.

**ASCII-MOS Approach:**

* `bo‘sh` -> `boesh`
* `bosh` -> `bosh`
* **Result:** Distinction preserved.

---
*This specification is dedicated to the public domain under CC0.*
