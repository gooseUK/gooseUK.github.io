
# Personal Website Specification

## Overview

Personal website for Brad Gooseman.

Purpose:

* Present professional experience and technical projects.
* Showcase systems architecture and engineering work.
* Publish technical articles and project postmortems.
* Provide CV and contact information.
* Act as a long-term archive of projects, lessons learned and technical writing.

The website should be static.

### Technology Stack

* Astro
* Tailwind CSS
* GitHub Pages
* GitHub Actions deployment

No backend.

No database.

No authentication.

---

# Design Goals

The design should be:

* Minimal
* Fast
* Technical
* Monospaced
* Professional
* Readable

Avoid:

* Glassmorphism
* Startup landing page aesthetics
* Excessive animations
* Skill bars
* Technology logo walls
* Marketing language
* "Graduate developer about-me" structure
  (Name → What I Do → Current Interests → Projects → Contact)
* Generic CV-style framing as the spine of the site

Inspiration:

* Technical documentation
* UNIX manuals
* Plain text websites
* Engineering notebooks
* Dot matrix printouts
* Fax paper textures

---

# Framing

The site is organised around systems design interests and
achievements — not around a personal profile.

The spine of the site is the work, the thinking, and the
cybernetic perspective behind both. Personal information
exists in service of that, not the other way around.

What this means in practice:

* Do not let the structure default to:
  Name → What I Do → Current Interests → Projects → Contact.
  That is the standard graduate-developer about-me pattern
  and the site should not read that way.
* Lead with systems, architectures, decisions, and the
  cybernetic frame. Let the personal details fall out of
  that context.
* "Name", "current role", "current interests", "contact" are
  still useful and should appear *somewhere* — but they are
  not the organising principle of the home page.
* Project writeups, architecture diagrams, postmortems, and
  the cybernetic essays are the load-bearing content.
* When in doubt: a senior systems engineer reading the home
  page should immediately see what kinds of systems I build
  and how I think about them — not learn my job title first.

This is a stylistic and structural rule, not just a copy
preference. Page hierarchy, home page sections, and
navigation order should all reflect it.

---

# Visual Style

## Colours

Background:

```css
#EEE7CF
```

Primary text:

```css
#111111
```

Secondary text:

```css
#444444
```

Very limited colour usage.

Mostly monochrome.

---

## Typography

Preferred fonts:

1. IBM Plex Mono
2. JetBrains Mono
3. Courier Prime
4. Courier New

Monospaced throughout.

---

## Layout

* Centered content column
* 800–1000px width
* Large margins
* Content-first design
* Navigation always visible

---

# Site Structure

## Home

Purpose:

Introduce who I am and what I work on.

Sections:

* Short introduction
* Current role
* Current interests
* Featured projects
* Recent articles
* Contact links

Suggested themes:

* Systems architecture
* Business software
* Automation
* Cloud infrastructure
* Distributed systems
* Robotics and software automation
* Cybernetics

---

## Cybernetic Perspective

A recurring intellectual thread across the site.

I approach business and software the same way I was trained to
approach control systems: as cybernetic processes with feedback
loops, sensors, actuators, controllers, and disturbances.

Most businesses are not described or run this way. Boards and
operational leaders tend to reason in terms of departments,
people, and goals — not in terms of loops, lag, signal, noise,
and stability. When I map a business this way, the structure
becomes obvious to me, but the framing is not natural to most
of the people I work with.

This site should make that perspective explicit:

* Reframe businesses as cybernetic processes rather than
  organisational charts.
* Identify the feedback loops that already exist (often
  implicit, often broken).
* Treat software systems as control surfaces for those loops.
* Use the language of control theory and cybernetics where it
  clarifies the engineering decisions.

Where it should appear:

* About — list cybernetics as a core influence on how I think.
* Articles — at least one article on reframing businesses as
  cybernetic systems.
* Project writeups — where relevant, surface the feedback loops
  the system was actually built to close.

This is not branding. It is the actual lens. The site should
read that way.

---

## Career Arc — Robotics to Business Software

The move from a Robotics & Mechatronics degree into business
software should not be framed as a pivot or a career change.

It should be framed as a continuation of the same scientific
interest — cybernetics — applied to a different substrate.

The throughline:

* Robotics is cybernetics applied to physical actuators.
* Business software is cybernetics applied to organisational
  actuators (people, processes, capital, information).
* The long-term interest is fully autonomous businesses:
  organisations whose internal control loops are closed in
  software rather than in meetings.

Intellectual lineage to draw on (in articles, About, and any
long-form writing):

* Norbert Wiener — foundational cybernetics, feedback,
  communication and control in the animal and the machine.
* Stafford Beer — management cybernetics, the Viable System
  Model, Project Cybersyn. The most direct precedent for
  treating a business as a controllable system.
* Kevin Kelly — *Out of Control*, the technium, emergent and
  decentralised systems.
* Nick Land — accelerationism, capital as a self-organising
  cybernetic process.
* CCRU (Cybernetic Culture Research Unit) — late-90s Warwick
  group treating culture, capital, and computation as one
  continuous cybernetic phenomenon.

This lineage is the explanation for why a roboticist ended up
building enterprise platforms: it is the same problem at a
different layer of the stack.

Where it should appear:

* About — short paragraph framing the transition this way.
* Articles — a long-form essay tracing the lineage and
  arguing for fully autonomous businesses as the logical
  endpoint.
* Possibly a dedicated reading-list / influences page if it
  grows large enough.

---

## About

Short professional background.

Topics:

* BSc Robotics & Mechatronics
* Software engineering career
* Lead Software Engineer at SECOM UK
* Focus on systems architecture, automation and business platforms

Avoid long biographies.

Keep concise.

---

## Projects

Primary portfolio section.

Each project should contain:

* Overview
* Problem statement
* Architecture
* Technologies used
* Screenshots
* Challenges
* Lessons learned
* Current status

### Project / Postmortem split

* `/projects/<name>` pages — **system synopsis**: technical run-down,
  architecture, technologies, design decisions.
* `/postmortems/<name>` pages — **operational story**: what
  actually happened in production, successes, failures, lessons.

The SYSTEMS list on the home page always links to the system
synopsis page (`/projects/<name>`), never directly to the
postmortem. The postmortem is reached from inside the system
page, or from the dedicated postmortems index.

### Pending project icons

Each project should have a small icon next to its title in
listings (home SYSTEMS, projects index, etc). User to provide
the assets; placement and styling to be defined when they
arrive.

* **Gnome Trader** — Old School RuneScape gold coin icon.
* **GnomeAIO** — Old School RuneScape levelling / xp icon.
* **SECOM Nexus** — red circle (SECOM brand mark).

These should be rendered small, monochrome where possible, and
sit inline with the title in a way that does not break the
man-page typographic feel.

---

### SECOM Nexus

Enterprise business platform.

Topics:

* FastAPI
* React
* PostgreSQL
* Google Cloud
* OAuth
* Event processing
* CAFM integrations
* Legacy system migration
* Internal business workflow automation

---

### GnomeAIO

Robotic automation platform for Old School RuneScape.

Topics:

* Software automation
* Bot orchestration
* Distributed task execution
* Queue management
* WebSockets
* Multi-client coordination
* Resource allocation
* Event-driven architecture

This project should be presented as an automation and orchestration system rather than simply a game bot.

---

### Gnome Trader

Automated trading platform built around the Solana ecosystem.

Topics:

* Trading automation
* Solana integration
* Strategy execution
* Monitoring
* Infrastructure
* Exchange integration
* Operational automation

Include screenshots and videos where available.

This project should also have a dedicated postmortem.

---

# Postmortems

Purpose:

Document lessons learned from completed or discontinued projects.

Each postmortem should contain:

* Executive summary
* Original thesis
* Architecture
* What worked
* What failed
* Root cause analysis
* Lessons learned
* What I would do differently

---

## Gnome Trader

Dedicated postmortem.

Topics:

* Original goals
* System architecture
* Development process
* Operational challenges
* Market assumptions
* Why the project failed
* Lessons learned

Include screenshots and embedded Wistia videos where available.

---

# Articles

Technical writing section.

Potential topics:

* Designing Event-Driven Business Systems
* FastAPI at Scale
* Internal Enterprise Software Development
* Robotic Automation and Orchestration Systems
* Lessons From Building Gnome Trader
* Designing Distributed Task Execution Platforms
* Cloud Architecture Lessons Learned

Goal:

A small collection of high-quality technical articles.

---

# CV

Simple page containing:

* Experience
* Education
* Skills
* Downloadable PDF CV

Implementation:

Store the PDF in:

```txt
public/cv.pdf
```

Provide links for:

* View CV
* Download CV

---

# Contact

Include:

* Email
* GitHub
* LinkedIn

Keep minimal.

---

# Media

Do not store videos in the repository.

Use external hosting:

* Wistia preferred
* YouTube optional

Embed videos using responsive iframes.

Example uses:

* Gnome Trader demonstrations
* GnomeAIO demonstrations

---

# Deployment

Repository:

gooseUK.github.io

Hosting:

GitHub Pages

Deployment:

GitHub Actions

Every push to main should automatically build and deploy the website.

---

# Guiding Principle

The website should emphasize:

* Systems built
* Problems solved
* Automation
* Architecture
* Technical decision making
* Lessons learned

The focus is on demonstrating engineering capability through real projects rather than listing technologies or making marketing claims.
