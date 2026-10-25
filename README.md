# BookEasy: Appointment Booking Demo

A front-end demo of an online appointment booking system for small clinics and salons. A visitor picks a service, a date and a time slot, enters their details, and confirms the booking.

**Live demo:** https://sahasranshu2339.github.io/Book-easy-demo/

## The problem

Small clinics and salons often take bookings by phone and WhatsApp. Slots get double-booked, customers forget their appointments, and staff spend time confirming and rescheduling by hand.

## What this demo shows

- Choose a service (consultation, follow-up or full check-up)
- Pick a date, with past dates blocked
- See time slots for that day, with already-taken slots disabled
- Enter a name and a phone number or email, with validation
- Instant confirmation message
- A list of upcoming bookings, sorted by date and time, with a cancel button
- Double-booking protection: a taken slot can't be booked again
- Bookings are remembered in your browser between visits
- Responsive layout, keyboard-friendly controls, and light and dark mode

## What this demo is not

This is a front-end prototype only. Be aware of these limits:

- There is **no backend or database**. Bookings are saved in your own browser (`localStorage`), so they are not shared between devices and disappear if you clear browser data.
- Some slots are shown as taken automatically, based on the date, to simulate a busy schedule.
- No emails or SMS reminders are sent. The confirmation message only shows what would be sent.
- There is no admin panel and no login.

## Tech stack

- HTML
- CSS (custom properties, grid layout, dark mode)
- Vanilla JavaScript (no libraries or build step)
- Browser `localStorage`

## Run it locally

No installation needed.

1. Download or clone this repo.
2. Open `index.html` in any browser.

## Deploy it

This repo is hosted with GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / root**.

## Planned full version

The production version of this idea would add a real backend:

- Django and Django REST Framework API
- MySQL database with a unique constraint on doctor, date and time to prevent double bookings at database level
- Staff admin panel to confirm, reschedule or cancel appointments
- Email reminders
- React or Django-template frontend connected to the API

These features are planned and **not built yet** in this repo.

## Author

**Sahasranshu Srichandan**
GitHub: [sahasranshu2339](https://github.com/sahasranshu2339)
Email: sahasranshu2329@gmail.com
Portfolio: https://sahasranshu2339.github.io/Portfolio/
