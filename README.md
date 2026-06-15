# VHire 🎮

> Bilingual fan session booking platform for indie VTubers — JP/EN

[![Status](https://img.shields.io/badge/status-in%20development-yellow)]()
[![Stack](https://img.shields.io/badge/stack-PHP%20%7C%20MySQL%20%7C%20JS-blue)]()
[![Language](https://img.shields.io/badge/language-JP%20%7C%20EN-red)]()
[![Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://gict.xsrv.jp/s_annese/vhire/public/)

---

## Overview

VHire is a school web project I started developing in January 2026.
It is a booking platform that connects fans with indie VTuber creators for one-on-one fan sessions.

The platform targets the Japanese market and is fully bilingual (Japanese / English), responsive, and mobile-friendly.

Inspired by platforms like Skeb, Fanicon, and Coconala — but focused specifically on VTuber fan session booking.

---

## Features

### Authentication
- Email login with 6-digit verification code
- Social login: Google OAuth 2.0
- Social login: LINE Login
- Social login: X (Twitter) OAuth 2.0

### Booking System
- VTuber profile pages with session types and availability
- Fan session booking flow
- Booking confirmation with email notification
- 24-hour reminder email before session
- Cancellation with modal + reason field + email notification
- Book Again shortcut from booking history

### Client Dashboard
- KPI cards (total bookings, upcoming sessions, completed sessions)
- Upcoming booking countdown
- Full booking history with status badges
- Favorite VTuber badge
- Japan-inspired UI layout

### VTuber / Creator Dashboard
- Creator profile editor
- Analytics (views, bookings, revenue overview)
- Availability and time-off management
- Booking management

### Favorites System
- Follow / unfollow VTubers
- In-app notifications for availability updates
- Email notifications for followed VTubers

### Discovery
- Browse page with search and tag filters
- Live vertical ticker with real VTuber data on homepage
- Tag system with Japanese translation
- How It Works page and FAQ page

### Additional
- Coupon / discount code system
- User review submission
- Contact form
- Admin panel
- Payment integration (in progress)

---

## Tech Stack

| Area | Technology |
|---|---|
| Backend | PHP 8.x |
| Database | MySQL |
| Frontend | HTML5, CSS3, JavaScript (vanilla) |
| Authentication | Custom email verification + OAuth (Google, LINE, X) |
| Email | PHP Mailer / SMTP |
| Local dev | XAMPP |
| Production hosting | Shared hosting (Japan — xsrv.jp) |
| Deployment | FileZilla (SFTP) |
| Version control | Git + GitHub (private repo) |

---

## Live Demo

🔗 [gict.xsrv.jp/s_annese/vhire/public/](https://gict.xsrv.jp/s_annese/vhire/public/)

> **Test credentials (client):** `client@example.com` / `password123`
> **Test credentials (VTuber):** `vtuber1@example.com` / `password123`

---

## Project Structure

```
vhire/
├── public/
│   ├── index.php        # Homepage with hero, ticker, about section
│   ├── browse.php       # VTuber discovery with filters
│   ├── book.php         # Booking flow
│   ├── dashboard.php    # Client dashboard
│   ├── auth.php         # Login / register
│   ├── auth-google-*    # Google OAuth flow
│   ├── auth-line-*      # LINE Login flow
│   ├── auth-x-*         # X (Twitter) OAuth flow
│   ├── verify.php       # Email verification
│   ├── profile.php      # VTuber public profile
│   ├── edit-profile.php # Creator profile editor
│   ├── analytics.php    # Creator analytics
│   ├── notification.php # In-app notifications
│   └── assets/          # CSS, JS, images
├── app/                 # Backend logic (helpers, config)
├── lang/                # Language files (JP/EN)
├── partials/            # Reusable PHP components
└── sql/                 # Database schema
```

---

## Security Note

> The source code of this project is currently **private**.

The codebase contains OAuth credentials (Google, LINE, X), database configuration, SMTP settings, and server-specific configuration.

This repository contains only the public showcase: README, feature list, and demo link.
The source code will be reviewed and published with all secrets removed at a later stage.

---

## Development Timeline

| Period | Milestone |
|---|---|
| January 2026 | Project start — basic booking flow, bilingual UI |
| February 2026 | Authentication system (email verification + OAuth) |
| March 2026 | Dashboard restyle, KPI cards, booking management |
| April 2026 | Favorites system, email notifications, Creator Tools |
| May 2026 | Performance optimizations (WebP -92%, minify CSS/JS, defer scripts) |
| June 2026 | Coupon system, reviews, contact form, ongoing improvements |
| Ongoing | Payment integration, public launch preparation |

---

## Status

Active development — School project (graduation: 2026)

Goal: Transform into a real product targeting the Japanese VTuber market post-graduation

---

*Developed by [Stefano Annese](https://github.com/AnneseStefano) — Kawasaki, Japan*
