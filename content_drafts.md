# Privacy Policy Draft

**Effective Date:** January 28, 2026

## 1. Introduction
Welcome to Klaviyo for Salla. Your privacy and the security of your data are our top priorities. This Privacy Policy explains how we handle merchant data and private keys.

## 2. Data Ownership
We believe that your data belongs to you. **We do not store any merchant data** (customer details, order history, etc.) on our servers. All event data captured from your Salla store is processed in real-time and passed through to Klaviyo.

## 3. Data Storage
- **Merchant Data:** Not stored on our infrastructure.
- **Private Keys:** To facilitate the integration, we store your Klaviyo Private API Key in a secure Firebase database. This key is used exclusively to authenticate requests to your Klaviyo account.
- **Mapping:** Private keys are mapped by your unique Merchant Store ID to ensure that event data is populated correctly for each individual store.

## 4. Security
Our infrastructure is built for security:
- **Server-Side Processing:** We use Google Tag Manager (GTM) server-side, hosted on Stape, to capture events from Salla webhooks.
- **Firebase Security:** Private keys are stored in a private, encrypted Firebase database with strict access controls.
- **Encrypted Transmission:** All data transmitted between Salla, our servers, and Klaviyo is encrypted using industry-standard protocols.

---

# FAQ Draft

### 1. How does the Salla-Klaviyo integration work?
The app uses a server-side Google Tag Manager (GTM) setup hosted on Stape. When an event occurs in your Salla store (like a new order), a webhook is sent to our secure server. We then use your Klaviyo private key (stored securely in Firebase) to send that event data directly to your Klaviyo account.

### 2. Is my data secure?
Yes. We do not store any of your merchant or customer data. We only store your Klaviyo Private API Key in a secure, private Firebase database to authenticate the connection. Our servers are hosted on Stape and use Firebase variables for secure data handling.

### 3. What marketing flows are supported?
The app supports a comprehensive range of marketing flows to help you grow your business:
- **Abandoned Cart:** Remind customers who added items to their cart but didn't finish.
- **Post-Purchase:** Send confirmation and follow-up emails immediately after an order.
- **Order Status Updates:** Automatically notify customers when their order is processing, shipped, or delivered.
- **Refund / Return:** Manage customer expectations during the return process.
- **Winback:** Target customers who haven't purchased in a while.
- **Repeat Purchase / Cross-Sell:** Recommend products based on previous purchases.
- **VIP Rewards:** Treat your highest-value customers with exclusive offers.
- **COD Confirmation:** Reduce cancellations for Cash on Delivery orders.
- **Coupon Tracking:** Monitor how your discount codes are performing.

### 4. Do I need to host anything?
No. Everything is managed through our server-side GTM and Firebase setup. You just need to connect your Salla store and provide your Klaviyo API credentials.
