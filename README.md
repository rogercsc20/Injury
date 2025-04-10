Injury-Free Marketplace & Dashboards

This repository houses the source code for our two-tier endurance athlete platform:

    Freemium Tier:

        Access to dashboards with Injury Risk and Recovery Scores.

        Pay-as-you-go for physiotherapy/massage sessions.

    Premium Subscription:

        All free features, plus 1 physiotherapy and 1 massage session per month (or equivalent credits).

        Additional advanced integrations (Garmin/Strava), deeper insights, and possibly more sessions.

Features Overview

    User Registration & Authentication

        Athletes can sign up for free or premium tiers.

        Providers (physios, massage therapists) can onboard with admin approval.

    Subscription Billing & Payments

        Stripe subscription for recurring payments.

        One-time payment for users in the free tier who need to book a session.

    Booking System

        Providers list availability.

        Athletes book sessions using either monthly credits (premium) or pay-per-visit (freemium).

    Injury-Prevention Engine

        Daily Check-In form (soreness, fatigue, sleep).

        Simple scoring logic for Injury Risk and Recovery Score.

        Dashboards to visualize trends.

    Admin Panel

        Approve providers.

        Manage subscription tiers.

        Track platform metrics (users, bookings, revenue).

Project Structure

.
├── backend
│   ├── app.py            # Flask app entry point
│   ├── requirements.txt  # Python dependencies
│   ├── Dockerfile        # Docker build for backend
│   ├── ...
├── frontend
│   ├── src/              # React (or Next.js) source code
│   ├── package.json      
│   ├── Dockerfile        
│   ├── ...
├── docker-compose.yml    # Brings up backend + frontend + DB
├── README.md             # You're reading it now!
└── ...
