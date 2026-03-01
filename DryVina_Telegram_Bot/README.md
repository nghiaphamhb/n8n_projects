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

## 🔄 Workflow Architecture

![Workflow Architecture](../assets/DryVina.png)


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
