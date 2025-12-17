# Graphical Password Authentication System

## Abstract

The **Graphical Password Authentication System** is an alternative authentication mechanism designed to overcome the limitations of traditional alphanumeric passwords. Instead of relying solely on text-based credentials, the system uses graphical elements such as images, CAPTCHA-based challenges, combined image–text passwords, and speech recognition techniques. The core idea is based on the psychological principle that humans can remember images more easily than text, thereby improving memorability while strengthening security against common attacks.

---

## Introduction

Authentication is a fundamental requirement in information security. Conventional text-based password systems suffer from several drawbacks, including poor memorability, password reuse across multiple platforms, and vulnerability to attacks such as brute force and dictionary attacks. Biometric systems, while more advanced, introduce issues such as spoofing and liveness detection.

Graphical password authentication provides a viable alternative by leveraging human visual memory. This project explores and implements multiple graphical authentication techniques and analyzes their effectiveness in terms of usability and security.

---

## Motivation

* Humans can recognize and recall images more easily than text strings.
* Graphical passwords are harder to crack using traditional password attacks.
* Reduces dependency on weak, reused, or easily guessable passwords.
* Enhances resistance to dictionary and brute-force attacks.

---

## Problem Statement

Traditional alphanumeric password-based authentication systems are insecure in practice. Users often choose weak passwords or reuse the same password across multiple platforms. Such practices make systems vulnerable to:

* Dictionary attacks
* Brute force attacks
* Guessing attacks

There is a need for a more secure and user-friendly authentication mechanism that improves memorability while providing stronger resistance to common attack vectors.

---

## Proposed System

The proposed system implements multiple authentication methods based on graphical and non-textual inputs. These methods can be used independently or in combination to enhance overall security.

---

## Methods & Algorithms

### 1. Image Sequence-Based Authentication

* Users are presented with a grid of images.
* Authentication is performed by selecting images in the correct predefined sequence.
* Images are repositioned on every login attempt to reduce shoulder-surfing attacks.
* Improves memorability and increases password space.

### 2. CAPTCHA Image-Based Authentication

* Uses image-based CAPTCHA challenges.
* Easier for humans to recognize compared to text CAPTCHA.
* Difficult for automated bots due to image recognition and semantic classification requirements.

### 3. Image + Text-Based Authentication

* Combines graphical elements with textual input.
* Easier for users to remember than pure text passwords.
* More resistant to automated attacks as it requires both image and text interpretation.

### 4. Hashing Algorithm: SHA-512/256

* Uses the SHA-512/256 hashing technique for secure password storage.
* SHA-512 output is truncated to 256 bits.
* More efficient on 64-bit architectures compared to SHA-256.
* Enhances security by ensuring that raw credentials are never stored.

### 5. Speech Recognition-Based Authentication

* Uses static text-dependent voice authentication.
* Users speak a predetermined passphrase during enrollment and verification.
* Adds an additional layer of authentication beyond visual input.

---

## Project Architecture

The system architecture consists of:

* User interface for graphical interaction
* Authentication logic layer
* Secure hashing and verification module
* Database for storing encrypted credentials

---

## Conclusion

Graphical password authentication schemes demonstrate better memorability and stronger resistance to major password attacks when compared to traditional text-based passwords. While many graphical authentication methods are still largely explored in academic and experimental environments, the results indicate that they offer a promising direction for future authentication systems.

The study concludes that graphical passwords provide a balanced improvement in both usability and security and can be further enhanced by integrating biometric techniques.

---

## Future Enhancements

* Integration with biometric authentication systems
* Advanced CAPTCHA image segmentation and object recognition
* Multi-factor authentication support
* Improved resistance to shoulder-surfing and spoofing attacks

---

## Authors

* Kaif Shaikh



---

## License

This project is developed for academic and educational purposes.

