# PatternGuard

PatternGuard is a cutting-edge security framework that identifies users not by what they know or what they have, but by how they behave.

By leveraging Deep Learning (PyTorch) and high-precision telemetry, PatternGuard analyzes the unique "rhythm" of a user's keystrokes, measuring micro-second variations to provide transparent, continuous authentication.

## AI

- **Model Architecture**: Designed and trained a Many-to-One LSTM network in PyTorch to handle variable-length typing sequences.

- **Feature Engineering**: Implemented data normalization and pre-processing for Dwell Time (Key Hold) and Flight Time (Key Interval) vectors.

- **Validation**: Utilized Self-Supervised Learning to build user-specific profiles with minimal labeled data.

- **Optimization**: Quantized the model for low-latency inference (<50ms) to ensure a seamless user experience.

## Cybersecurity

- **Anti-Tampering**: Developed a signature-based validation system using HMAC-SHA256 to ensure telemetry data integrity.

- **Privacy Engineering**: IThe system processes timing patterns without ever storing the actual keys pressed (preventing keylogging).

- **Threat Modeling**: Conducted "Mime Attacks" to test model robustness against adversarial imitation.

- **Secure Infrastructure**: Configured JWT-based session management and implemented Rate Limiting to mitigate brute-force attempts on biometric patterns.
