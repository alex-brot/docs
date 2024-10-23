---
title: Container Shop System
weight: 3
---

# Alex-Brot Container-Shop-System

## Existing Local Systems

Tested existing shop systems from similar businesses to explore different functioning options.

- Off-Grid Saleshut (Yard Shop ~Innertreffling)
  - cash payment only
  - always open
  - no internet, no power
  - trust based - no further security measures
- Bio Bauer in Mittertreffling
  - cash payment only
  - no internet, no power
  - with seller on site or 24/7 shop
  - trust based - no further security measures
- Yard Shop (~Altenberg)
  - cash payment only
  - always open
  - Access Control with Credit Card


## Payment Options

- **SumUp**
  - Terminal Price: 25€
  - Fees: 1.69% per transaction
  - Android Tap To Pay: ✔️

- **Stripe**
  - Terminal Price: 59$
  - Fees: 1.5% + €0.25 per transaction
  - Android Tap To Pay: ✔️

- **PayPal**
  - Terminal Price: 29$
  - Fees: 2.29% + $0.09 per transaction
  - Android Tap To Pay: ✔️

## Internal Payment & Access System
- **Additional ESP8266/ESP32 for Payment**
  - Bar/QR/NFC code scanning for Products
  - Working with Payment Integration for seamless operation.
  - Alternative: Manual input of payment

## Access Control Options
- **Code Access (PIN/via Web-App)**
  - Users gets a PIN or can unlock via the web-app.
  - Cons: Requires user to have access to the app; limited security.
  
- **NFC**
  - Implement NFC access with a tag or phone.
  - Cons: Limited to NFC-enabled devices / needed tags

- **Unlock via Web-App**
  - Users can unlock via the web-app.
  - Cons: Requires user to have access to the app; limited security.

- **Video/Photo Logging (ESP-CAM)**
  - Capture a photo or video of users accessing the container for added security.
  - Store the footage temporarily and overwrite older data.
  - Cons: additional hardware (but should be cheap)

## Conclusion
Setup:
1. **Access Control:** NFC access with ESP8266 combined with video logging for security.
2. **Payment:** SumUp for cost-effectiveness. - For Testing Android Tap To Pay
3. **Internal Payment:** A second ESP8266/ESP32 to manage card/mobile payments inside.
