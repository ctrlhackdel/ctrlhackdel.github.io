---
title: Administrator Dashboard Project Structure
parent: Tech Stack and Project Structure
nav_order: 3
layout: default
---
# Administrator Dashboard Project Structure
This repository was reused between 2024 and 2025, only needing to be restructured to handle Postgres rather than MySQL. Most of the underlying framework was originally forked from the 2024 dashboard.
```
admin-cdh/
├── actions/                # Predefined scripts that can run independently
├── app/                    # Main app pages
│   ├── api/                # API routes
│   ├── hackers/            # Pages related to the hackers table
│   ├── logs/               # JSON recorded logs that track activity.
│   ├── role-management/    # List of administrator users
│   ├── sign-in/            # Sign in page - uses routing from existing db betterauth
│   ├── statistics/         # Graphs on database statistics
│   ├── test-email/         # View email preview
│   └── users/              # Pages related to the users table
├── components/             # Charts, Reusable components and Emails
├── data/                   # ORM-related queries
├── hooks/                  # Hooks related to client-side activities
├── lib/                    # Fonts, database schemas, etc.
├── public/                 # Images
├── scripts/                # Actions that can be executed outside of the client, usually DB related
└── types/                  # Interfaces and enumerations
```