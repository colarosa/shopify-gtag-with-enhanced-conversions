# Google Ads Conversion Tracking for Shopify (with/enhanced conversions)

## Overview

This script integrates Google Ads conversion tracking into an e-commerce platform. It tracks key checkout events (`checkout_started` and `checkout_completed`), ensuring that conversion data is sent to Google Ads for accurate attribution and performance measurement.

## Features

- Tracks **Checkout Started** (`checkout_started` event)
- Tracks **Checkout Completed** (`checkout_completed` event) and sends conversion data
- Dynamically loads Google Ads tracking script
- Supports **Enhanced Conversions** (email and phone) for better attribution
- Sends transaction details, including:
  - Total price
  - Currency
  - Transaction ID

## Installation

1. Copy and Paste this code into the customer events section of your Shopify Store. Bavigate to tge admin area to find this section.
2. Replace `XXXXXXXX` and `XXXXXXXXXXXX` with your **Google Ads Conversion ID** and **Conversion Label**.
3. Ensure that your project includes an `analytics` event system that triggers `checkout_started` and `checkout_completed`.
4. Add the script to your checkout page or global JavaScript bundle.

## Configuration

Modify the following lines with your actual Google Ads credentials:

```javascript
const conversionID = "XXXXXXXX"; // Replace with your Google Ads Conversion ID
const conversionLabel = "XXXXXXXXXXXX"; // Replace with your Google Ads Conversion Label
