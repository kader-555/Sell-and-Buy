# Sell-and-Buy
Sell&amp;Buy: a full-stack online marketplace where people can buy and sell products. Django REST API, React web app, Flutter mobile app, PostgreSQL.
# Sell&Buy

Sell&Buy is a full-stack online marketplace where individuals and small
businesses can sell products and buyers can discover, order, and receive
them in one place.

> 🚧 Status: in development (design and requirements phase)

## Problem

Buying and selling through social media groups and informal channels is
risky and disorganized: no order tracking, no structured catalog, no seller
reputation, and no protection against scams.

## Solution

A centralized platform with structured product listings, search and
filtering, a managed order lifecycle, seller ratings, and admin moderation.
A later phase adds an **escrow payment system** that holds the buyer's
payment until delivery is confirmed.

## Features

### MVP
- Registration and authentication (buyer and seller roles)
- Product listings with photos, price, category, and description
- Browse, search, and filter
- Shopping cart and order placement
- Seller dashboard for managing products and orders
- Order status tracking
- Admin panel for moderating users and listings

### Planned
- Ratings and reviews
- Buyer-seller messaging and notifications
- Escrow payments with delivery confirmation, auto-release timer,
  and dispute handling

## Tech Stack

| Layer    | Technology                          |
|----------|-------------------------------------|
| Backend  | Django, Django REST Framework       |
| Database | PostgreSQL                          |
| Web      | React.js                            |
| Mobile   | Flutter                             |
| Auth     | JWT                                 |
| API docs | OpenAPI (drf-spectacular)           |

## Architecture

A modular monolith: one Django backend serving both clients through a
REST API.

```
React (web)  ─┐
              ├──► Django REST API ──► PostgreSQL
Flutter (app) ─┘
```

## Project Structure

```
sell-and-buy/
├── backend/    # Django REST API
├── frontend/   # React web app
├── mobile/     # Flutter app
└── docs/       # Vision, requirements, design documents
```

## Documentation

- [Vision](docs/01-vision.md)
- [Requirements](docs/02-requirements.md)

## Getting Started

Setup instructions will be added as development progresses.

## Roadmap

- [ ] Requirements and design (ERD, order state machine)
- [ ] Backend: authentication and user roles
- [ ] Backend: products, cart, orders
- [ ] React web app (MVP)
- [ ] Flutter mobile app (core flow)
- [ ] Reviews, messaging, notifications
- [ ] Escrow payment system

## Author

Mouhamed Abdelkader 17/10/2026
