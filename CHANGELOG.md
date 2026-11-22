# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 72,606 endpoints from 5,304 services, tested 14–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 67,965 endpoints from 4,793 services, 4,641 fewer endpoints than first published under this snapshot (72,606 from 5,304 services), tested 14–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Energy_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 67k-energy-apis-for-agents (was 72k-energy-apis-for-agents; first published as energy-api-endpoints). The name follows the count, rounded down.
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
