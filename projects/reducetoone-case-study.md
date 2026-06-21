# ReduceToOne — Private-Code Product Case Study

ReduceToOne is a private-code product focused on centralizing important calendar and community event information from user-connected sources.

The core idea is simple: people miss important events, deadlines, and updates because information is scattered across calendars, social posts, emails, group pages, and organization announcements. ReduceToOne is designed to reduce that noise into one clearer place to check what matters.

## My Role

Founder and developer.

I am responsible for product direction, implementation, integration planning, data modeling, and the security/privacy decisions around connected user information.

## Problem

Students and communities often rely on fragmented sources:

- personal calendars
- Google Calendar events
- forwarded emails
- Facebook Pages
- Instagram Business posts
- GroupMe groups
- organization pages and shared sources
- manual announcements

The result is not just inconvenience. Important events and action items can be missed because the information is spread across too many places.

## Product Direction

ReduceToOne is being built as a dashboard and calendar layer for high-signal events and action items.

The product focuses on:

- bringing relevant events into one daily brief
- letting users subscribe to trusted groups and sources
- supporting personal and community calendars
- giving users control over what appears in their calendar
- using AI-assisted extraction carefully, with review and trust gates
- avoiding false positives when information is ambiguous

## Technical Stack

- Next.js / React / TypeScript
- Tailwind CSS
- Prisma
- Supabase Postgres
- Clerk authentication
- Vercel deployment
- API-based integrations
- AES-256-GCM encryption for OAuth token storage

## Security and Privacy Considerations

ReduceToOne handles connected-source data, which makes privacy and trust central to the design.

Important security considerations include:

- encrypted OAuth token storage
- account and group-level permission boundaries
- source trust controls
- cautious event extraction and review queues
- avoiding automatic creation from weak or ambiguous evidence
- audit logging for important actions
- clear separation between deterministic app behavior and AI-assisted parsing

## AI / Extraction Design

The extraction system is designed around a precision-first rule:

> A false event can be more harmful than a missed event.

That means the system should prefer review, evidence, and confidence checks before auto-publishing extracted events.

The extraction direction includes:

- event-worthiness classification before extraction
- structured extraction instead of freeform AI output
- validator gating for dates, titles, times, and locations
- evidence-backed fields
- duplicate detection
- review outcomes and rollback paths
- source-specific handling for social posts, flyers, emails, and manual text

## Why the Code Is Private

The source code is private because the project includes proprietary product direction, integration architecture, and security-sensitive implementation details.

A live walkthrough, architecture review, or time-boxed code review can be made available on request.

## What This Project Demonstrates

ReduceToOne demonstrates:

- security-minded product development
- SaaS architecture and data modeling
- connected account and API integration planning
- privacy-conscious handling of user-connected information
- AI-assisted extraction with responsible guardrails
- practical product thinking beyond a class assignment

## Current Status

Active build.

The project is being developed as a real product, with cybersecurity, software engineering, and responsible AI concerns treated as core design constraints rather than afterthoughts.
