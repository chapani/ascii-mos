# ASCII-MOS 🌍

**ASCII-MOS** is an ASCII-safe transliteration standard for the Uzbek language, designed for programming identifiers, URLs, and database keys.

## Why ASCII-MOS?

Standard Uzbek Latin characters like `o'` and `g'` are problematic in code. Stripping them often leads to semantic collisions (e.g., both "convert" and "heavy" becoming `ogir`). ASCII-MOS uses "Safe" (Omon) digraphs to preserve meaning and logic.

## Resources

- [Technical Specification (English)](docs/SPEC_EN.md)
- [Uzbek Main Page](README.md)
- [EXAMPLES in Uzbek](docs/EXAMPLES.md)
- [Machine-readable Rules (JSON)](data/rules.json)

## License

This work is dedicated to the public domain under **CC0 1.0**. You are free to use, modify, and distribute this standard without any restrictions or attribution requirements.
