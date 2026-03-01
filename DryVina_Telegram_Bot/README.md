# DryVina Telegram Sales Bot

This project is an **AI-powered Telegram sales assistant** built with n8n.
It helps automate customer interactions for a dry food shop (DryVina), including product inquiries, stock checking, and order handling.

---

## 📌 Overview

This workflow connects **Telegram + AI (LLM) + Google Sheets** to create a smart chatbot that can:

* Understand user intent (buy, check stock, ask for products)
* Match requested products with inventory
* Respond naturally in a friendly conversational tone
* Assist with simple order flows

---

## 🧠 Features

### 1. Intent Detection (AI)

* Uses LLM to classify user messages into:

  * `buy`
  * `check_stock`
  * `list_products`
  * `other`

### 2. Product Extraction

* Extracts product names and quantities from messages
* Supports multiple products in one request

### 3. Smart Matching System

* Fuzzy matching using:

  * Text normalization (Vietnamese-friendly)
  * Token comparison (Jaccard similarity)
* Handles:

  * Typos
  * Different naming formats

### 4. Inventory Integration

* Connects to Google Sheets as a product database
* Reads:

  * Product name
  * Stock quantity
  * Unit

### 5. Conversational AI Replies

* Generates natural responses:

  * Friendly tone ("tớ – cậu")
  * Context-aware replies
  * Handles edge cases (out of stock, unclear requests)

### 6. Telegram Automation

* Fully automated message handling
* Sends responses directly back to users

---

## 🧩 Main Components

| Component         | Description                                |
| ----------------- | ------------------------------------------ |
| Telegram Trigger  | Receives incoming messages from users      |
| LLM Intent Parser | Converts user message into structured JSON |
| Google Sheets     | Stores product inventory                   |
| Matching Engine   | Matches user input with real products      |
| AI Reply Composer | Generates human-like responses             |
| Telegram Send     | Sends final response back to user          |

---

## 📝 Notes

* Designed for Vietnamese language input
* Optimized for conversational commerce
* Easily extendable for:

  * Payment integration
  * Order tracking
  * CRM systems
