# Secure-IT

Secure-IT is an iOS security application designed to validate encrypted event tickets in real time using QR-based cryptography. The project was built as a fraud-prevention solution for event access control and won **1st Place at ENACTUS 2025** out of 30+ teams.

## Overview

Event ticket fraud can create financial losses, security risks, and poor user experiences for organizers and attendees. Secure-IT addresses this problem by using encrypted QR codes and a lightweight verification pipeline to confirm ticket authenticity quickly and reliably.

The application allows event staff to scan encrypted tickets, verify them against backend records, and determine whether a ticket is valid, invalid, duplicated, or already used.

## Features

- Encrypted QR-based ticket validation
- Real-time ticket verification
- iOS mobile scanning interface
- Firebase backend integration
- Secure ticket status tracking
- Duplicate ticket detection
- Fast verification pipeline
- Team-based MVP developed under competition constraints

## Tech Stack

**Mobile**
- Swift
- SwiftUI
- CryptoKit
- AVFoundation

**Backend / Cloud**
- Firebase
- Firestore
- Firebase Authentication

**Security**
- QR-based cryptography
- Encrypted ticket payloads
- Ticket validation logic

**Tools**
- Xcode
- Git
- GitHub

## Project Highlights

- Built an end-to-end iOS security app using Swift, CryptoKit, Firebase, and QR-based cryptography.
- Designed a verification pipeline capable of processing **500+ scans per minute** with **<150ms latency**.
- Created a real-time validation flow for encrypted event tickets.
- Led a 4-person engineering team from concept to fully functional MVP.
- Won **1st Place at ENACTUS 2025** out of 30+ teams for social and technical impact.

## How It Works

1. A ticket is generated with an encrypted QR payload.
2. Event staff scans the QR code using the iOS app.
3. The app decrypts or validates the ticket payload.
4. Firebase is queried to check the ticket status.
5. The app displays the result:
   - Valid
   - Invalid
   - Already used
   - Duplicate
6. If valid, the ticket status is updated to prevent reuse.
