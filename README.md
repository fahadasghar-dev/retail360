<p align="center">
  <img src="https://img.shields.io/badge/Oracle-APEX-F80000?style=flat&logo=oracle&logoColor=white">
  <img src="https://img.shields.io/badge/PL%2FSQL-Oracle-F80000?style=flat&logo=oracle&logoColor=white">
  <img src="https://img.shields.io/badge/Cloud-OCI-C74634?style=flat&logo=oracle&logoColor=white">
  <img src="https://img.shields.io/badge/AI-Claude-D97757?style=flat&logo=anthropic&logoColor=white">
  <img src="https://img.shields.io/badge/Tests-Playwright-2EAD33?style=flat&logo=playwright&logoColor=white">
  <img src="https://img.shields.io/badge/Status-in%20real%20use-0A3E30?style=flat">
</p>

# Retail360

A point-of-sale and store app for **marts, pharmacies and grocery stores** in Pakistan.
Fast barcode billing at the counter, stock with expiry dates, a store map of racks and shelves, purchases, cash, staff salary and reports,
in one app for laptop and phone, in English and Roman Urdu, light and dark mode.

This repository is a project showcase (screens and features). The source code is private.

## Screens

From the demo mart (sample data only).

| Dashboard | POS (counter billing) |
|---|---|
| ![Dashboard](screens/dashboard.png) | ![POS](screens/pos.png) |

| AI assistant | Store map (shelf view) |
|---|---|
| ![AI assistant](screens/ai_assistant.png) | ![Store map](screens/store_map.png) |

| Store map: refill list | Store map: refill shelves |
|---|---|
| ![Refill list](screens/store_map_refill_list.png) | ![Refill shelves](screens/store_map_refill_shelves.png) |

## What it does

- **POS:** barcode scan or name search, keyboard shortcuts, hold and recall bills, discounts, cash / card / credit (khata), split payment, printed receipts
- **Stock:** items with expiry dates, low-stock and near-expiry alerts, stock audit by scanning, barcode label printing
- **Store map:** racks and shelves drawn as a map; find any item, see what is out of stock or expired on which shelf, refill list
- **Purchases:** supplier bills, returns, last purchase price and stock in hand while buying
- **Cash:** cash drawer per counter, day start and day close (Z-report), expenses, matching cash
- **Customers:** khata (credit) accounts, payments and reminders
- **Staff:** employees, advances and monthly salary sheet
- **Reports:** sales, profit and margin, top sellers, stock worth, expiry
- **AI assistant:** answers questions like "What sold the most this week?" from the mart's own data; read-only, and only what the user's role is allowed to see
- **Multi-counter and roles:** several counters at once; owner, manager and cashier roles with permissions

## How it is built

- **Oracle APEX** (native components) on **Oracle Database**, business rules in **PL/SQL** packages
- **Multi-tenant:** many marts on one system; every mart sees only its own data
- **Oracle Cloud (OCI)** hosting
- **AI assistant:** LLM (Claude) with read-only tools written in PL/SQL, checked against the user's shop and permissions
- **Playwright** end-to-end tests on laptop and phone sizes, English and Roman Urdu

## Contact

Fahad Asghar · Senior Oracle APEX Developer
[LinkedIn](https://www.linkedin.com/in/fahad-asghar25) · [kafacloud.com](https://kafacloud.com) · kafacloud.info@gmail.com
