## Energy API endpoints, snapshot 15 Nov 2026

- 67,965 endpoints passed a keyless data call, tested 14–15 Nov 2026 (IST)
- 4,793 services · 251 country codes · 46,598 keyless JSON rows

### Download

- `Energy_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 67,965 rows, 2.3 MB gzipped (18.9 MB as CSV), SHA-256 `01a6548ec764a5fafc81a8ff444426dce85a5d1571644f48e9b476cb370f9934`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Energy_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Energy_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 418 · Wrap one URL pattern as a get_power_mix or get_power_price tool: pass a country, bidding zone or region, return generation by source, the price or the carbon intensity with its timestamp; add a timeout.
- 📱 App features: 6,803 · Show power plants, solar and wind sites, substations, chargers or fuel stations near a place on a map; each layer query returns features with names, capacities or fuel types.
- 🧠 Grounding and data pipelines: 23,784 · Load energy balances, generation, consumption and price series on a schedule into your own store, so answers about a country's energy cite a dated source.
- 🧪 Evals and testing: 67,965 · Run your energy tool against a fixed set of URLs across formats; check that units (MW, MWh, price per MWh, gCO2/kWh), timestamps and country codes parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release: 72,606 endpoints from 5,304 services, tested 14–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 67,965 endpoints from 4,793 services, 4,641 fewer endpoints than first published under this snapshot (72,606 from 5,304 services), tested 14–15 Nov 2026 (IST).
- Left out: 635 rows whose URL carried a credential-looking parameter or a login.
- Left out: 2 rows with an email-like address.
- Left out: 399 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 3 layers marked editable in the title (they can hold entries that people added).
- Left out: 50 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 352 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 14 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Left out: 5 ArcGIS layers that are records about named people (employee, patient, client or donor lists, home addresses, voter lists, sex offender and missing person layers).
- Left out: 1 row that is another address of an ArcGIS layer dropped for what it holds (one of the reasons above, found under another address of the layer).
- Left out: 83 rows of ArcGIS Online organisations that are class accounts (25 layers or more, at least 50% of them class or coursework layers): their other layers are students' work too.
- Left out: 1,497 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 268 rows of class sets: one map layer saved under 5 or more students' initials or names in one ArcGIS Online organisation, or in 4 or more students' own organisations.
- Left out: 3,190 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
- Left out: 39 rows that repeat an address already in the pack.
- Left out: 43 rows whose title is about COVID-19 or vaccination (map layers filed under energy, not about energy).
- Overlap: 2,652 of these URLs are also in 170k-weather-apis-for-agents.
- Overlap: 139 of these URLs are also in 240k-transit-apis-for-agents.
- Overlap: 200 of these URLs are also in 260k-water-apis-for-agents.
- Overlap: 1,414 of these URLs are also in 120k-finance-economy-apis-for-agents.
- Overlap: 54 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 144 of these URLs are also in 1.2m-government-open-data-apis.
- Overlap: 5 of these URLs are also in 270k-statistics-apis-for-agents.
- Overlap: 64 of these URLs are also in 84k-oceans-apis-for-agents.
- Overlap: 9 of these URLs are also in 160k-environment-apis-for-agents.
- Overlap: 115 of these URLs are also in 19k-air-quality-apis-for-agents.
- Overlap: 65 of these URLs are also in 350k-maps-gis-apis-for-agents.
- Overlap: 46,465 of these URLs are also in 2.2m-agent-ready-apis.
- Overlap: 5 of these URLs are also in 380k-science-apis-for-agents.
- Overlap: 1 of these URLs is also in 40k-hazards-apis-for-agents.
- Overlap: 1 of these URLs is also in 4.9k-wildfire-apis-for-agents.
- Overlap: 15 of these URLs are also in 22k-traffic-apis-for-agents.
- Overlap: 1 of these URLs is also in 7.8k-earthquake-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 14–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Energy API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
