# CV — Experience section (current state)

Current state of the `\section{    Experience}` block as authored in Overleaf.

Order: SECOM → British Steel → Lampada → E.ON → Gnome Trader (Personal Project at the bottom).

```latex
\section{    Experience}
    \resumeSubHeadingListStart
        \resumeSubheading
          {Lead Software Engineer}{Sep. 2024 -- Present}
          {SECOM Plc}{}
          \resumeItemListStart
            \resumeItem{Technical lead building a new business platform for both internal and customer use with Python, FastAPI, React, TypeScript, and Redis.}
            \resumeItem{Designed and built event-driven backend services that synchronise operational data across on-premises and third-party systems.}
            \resumeItem{Migrating legacy MySQL platforms onto a unified service-based architecture without downtime.}
            \resumeItem{Replacing manual workflows and document generation across the organisation.}
            \resumeItem{Own architecture, CI/CD, and operational reliability across all services on Google Cloud.}
          \resumeItemListEnd
        

        \resumeSubheading
          {Systems Engineer}{Jan. 2024 -- Sep. 2024}
          {British Steel}{}
          \resumeItemListStart
            \resumeItem{Designed a molten steel tracking system to capture material used and wasted across the plant.}
            \resumeItem{Built data pipelines combining Digital Matter GPS telemetry, on-site sensor feeds, and legacy systems to support real-time logistics and production decisions.}
            \resumeItem{Interfaced with legacy Fortran and COBOL systems running critical production and financial reporting workflows.}
            \resumeItem{Built datasets used by operations for cost tracking, efficiency analysis, and production optimisation.}
          \resumeItemListEnd
        

        \resumeSubheading
          {Software / Electronics Engineer}{Jun. 2022 -- Jan. 2024}
          {Lampada}{}
          \resumeItemListStart
            \resumeItem{Built a GPS-based campus navigation app for the University of Hull, with pathfinding around campus buildings and walkways.}
            \resumeItem{Designed and prototyped custom PCBs for client projects, from schematic capture through layout to manufacture.}
          \resumeItemListEnd
        

        \resumeSubheading
          {Hydraulics Technician}{May 2018 -- Sep. 2019}
          {Siemens Gamesa}{}
          \resumeItemListStart
            \resumeItem{Built, calibrated, and serviced high-pressure hydraulic systems and devices used across the wind turbine industry.}
          \resumeItemListEnd
        

        \resumeSubheading
          {Offshore Wind Turbine Technician}{Sep. 2015 -- May 2018}
          {E.ON Energy}{}
          \resumeItemListStart
            \resumeItem{Hands-on mechanical, electrical, and hydraulic maintenance of offshore wind turbines, with direct responsibility for turbine availability and generation uptime.}
            \resumeItem{Fault diagnosis and resolution using SCADA telemetry and on-site instrumentation across power generation, control, and safety systems.}
            \resumeItem{Worked under strict safety, working-at-height, and offshore-access certifications (GWO standards) in a remote, weather-constrained operational environment.}
          \resumeItemListEnd
        
        \resumeSubheading
          {Software Engineer}{Mar. 2024 -- Jan. 2026}
          {Gnome Trader (Personal Project)}{}
          \resumeItemListStart
            \resumeItem{Reduced end-to-end delivery latency from approximately one hour of manual processing to sub-20-second automated execution.}
            \resumeItem{Designed and built a distributed Solana payment and delivery platform. Python, FastAPI, WebSockets, Redis, PostgreSQL, atomic Lua-scripted Redis claims with TTL self-healing.}
            \resumeItem{Verified on-chain Solana transactions before triggering downstream fulfilment, with idempotent payment processing and tolerance-window amount matching.}
          \resumeItemListEnd
        \resumeSubHeadingListEnd
```

## Section structure changes vs the earlier version of this file

- **Order on the page**: Education now sits above Experience (was the other way around).
- **Header**: now reads `gooseman.uk | brad_gooseman@hotmail.com | linkedin.com/in/brad-gooseman-8788a6241/ | github.com/gooseUK` on the top line, with the phone number `+44 7429 316 117` on a second centered line beneath.
- **Core Technical Focus**: removed entirely. Tech keywords now live inline in the experience bullets.
- **E.ON role title**: changed from `Offshore Wind Turbine Engineer` to `Offshore Wind Turbine Technician`.
- **Lampada dates**: `Jun. 2022 -- Jan. 2024` (continuous from graduation through to British Steel).
- **British Steel molten steel bullet**: tightened to `Designed a molten steel tracking system to capture material used and wasted across the plant.` (the earlier double-`used` is gone).
- **SECOM lead bullet**: now uses the Oxford comma — `Python, FastAPI, React, TypeScript, and Redis`.

Both of the previously-flagged typos (the `Built  data pipelines` double space, and `PCB's` apostrophe) are now fixed.
