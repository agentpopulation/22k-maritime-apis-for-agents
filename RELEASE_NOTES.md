## Maritime API endpoints, snapshot 15 Nov 2026

- 22,485 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 3,117 services · 71 country codes · 12,206 keyless JSON rows

### Download

- `Maritime_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 22,485 rows, 1.1 MB gzipped (6.6 MB as CSV), SHA-256 `3cfb6e8800ef1b094a8b2a33a7e07ab5f91ccd5c333aec2ef20f2da1207867b9`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Maritime_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Maritime_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 4,326 · Wrap the port-call URL as a get_port_calls tool: pass a UN/LOCODE port code (FIHEL), return the ships with arrival and departure times; add a timeout.
- 📱 App features: 4,349 · Show ports, ferry piers, moorings and harbour limits on a coastal map card, with the layer name and the date it passed.
- 🧠 Grounding and data pipelines: 1,390 · Load freight, port-call and ship-count tables on a schedule into your own store, so answers about port traffic cite a dated table.
- 🧪 Evals and testing: 22,485 · Run your maritime tool against a fixed set of URLs across formats; check that port code, ship name, time or feature geometry parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 24,827 endpoints from 3,457 services, tested 10–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 22,485 endpoints from 3,117 services, 2,342 fewer endpoints than first published under this snapshot (24,827 from 3,457 services), tested 10–15 Nov 2026 (IST).
- Left out: 4 rows with an email-like address.
- Left out: 235 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 23 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 140 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 18 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 4 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 4 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 583 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 39 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 1,662 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 23 rows that repeat an address already in the pack.
- Overlap: 468 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 1,836 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 3,039 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 64 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 15 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 42 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 2 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 2,461 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 1 of these URLs is also in 160k-environment-apis-for-agents.
- Overlap: 122 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 17 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 12,188 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 1 of these URLs is also in 84k-health-apis-for-agents.
- Overlap: 2 of these URLs are also in 40k-hazards-apis-for-agents.
- Overlap: 4 of these URLs are also in 4.9k-wildfire-apis-for-agents.
- Overlap: 2 of these URLs are also in 23k-aviation-apis-for-agents.
- Overlap: 1,293 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 58 of these URLs are also in 10k-parking-apis-for-agents.
- Overlap: 109 of these URLs are also in 7.8k-earthquake-apis-for-agents.
- Overlap: 26 of these URLs are also in 4.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Maritime API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
