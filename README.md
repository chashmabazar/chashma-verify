# Chashma Bazar — Official Invoice Verification Portal

> **Trusted Companion of Your Eyes**

The official QR-based digital invoice verification portal for **Chashma Bazar**. Customers and staff can scan the QR code printed on any official Chashma Bazar A5 invoice to verify live order status, itemized billing, optical prescription (Rx), payment balance, and delivery audit details in real time.

---

## Key Features

- **Instant QR Verification:** Scan any official invoice QR code to load verified order details directly in the browser.
- **Tamper-Resistant Security:** Protected by per-invoice cryptographic verification tokens (`HMAC-SHA256`) to prevent unauthorized access or invoice number guessing.
- **Live Order & Delivery Audit:** Displays real-time order status (`PROCESSING`, `READY`, `DELIVERED`), payment mode, prepared by, and delivery timestamps.
- **Itemized Billing & Rx Summary:** Shows multi-item frame/lens breakdowns, discounts, advance payments, balance due / `FULL PAID` status, and optical prescription (`OD`/`OS` & `IPD`).
- **Fast & Reliable Architecture:** Hosted on GitHub Pages with dual-transport API failover (`fetch` + sanitized `JSONP`) and session caching for fast mobile loading.

---

## How It Works

1. An order is created or updated in the **Chashma Bazar Optical ERP** Android app.
2. The backend generates an official A5 PDF invoice embedded with a unique, token-secured QR code.
3. Scanning the QR code opens this portal (`https://chashmabazar.github.io/chashma-verify/?inv=CB-XXX&t=TOKEN`) and validates the record live against official store records.

---

## Store Information

- **Brand:** Chashma Bazar
- **Address:** Sawkat Bhabon, 94 New Elephant Road, Dhaka, Bangladesh
- **Hotline:** +880 1644-138132

---

*© 2026 Chashma Bazar. All rights reserved.*
