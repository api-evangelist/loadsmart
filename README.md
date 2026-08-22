# Loadsmart (loadsmart)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Loadsmart is a digital freight technology company and 4PL that connects shippers, carriers, warehouses, and dock operations on a single platform. Founded in 2014 by Felipe Capella and Ricardo Salgado and headquartered in Chicago (with significant New York presence), Loadsmart raised more than $346M from investors including BlackRock, SoftBank Latin America Fund, Maersk Growth, TFI International, CSX, Ports America, and Connor Capital, reaching a reported $1.3B valuation. The platform spans full and partial truckload, less-than-truckload, drayage, expedited, flatbed (via Flatbed Messenger), and multimodal freight, plus the ShipperGuide TMS for procurement, planning, and execution; CarrierGuide TMS and a carrier loadboard with factoring; Opendock for dock appointment scheduling and the Nova warehouse API; and NavTrac for yard management and computer-vision gate/yard visibility. FreightIntel AI provides machine-learning powered freight recommendations across the suite. Loadsmart exposes a public Developer Portal with two production OpenAPI surfaces — the ShipperGuide API (api.loadsmart.com, JWT/RS256 authentication, with quote, book, tender, track, and webhook lanes) and the Opendock Nova / Neutron API (neutron.opendock.com, JWT bearer authentication) — and ships a Postman collection plus partner integrations with Oracle Transportation Management, MercuryGate, Blue Yonder, SAP, NetSuite, and other TMS/ERP platforms.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/loadsmart/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Producing
- **Access:** 3rd-Party

## Tags

- Freight
- Logistics
- Transportation
- Supply Chain
- Digital Freight
- Freight Brokerage
- Truckload
- LTL
- Drayage
- Flatbed
- Multimodal
- TMS
- Dock Scheduling
- Yard Management
- Warehouse
- 4PL
- FreightTech

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Loadsmart ShipperGuide API

Production REST API at https://api.loadsmart.com (sandbox api.sandbox.loadsmart.com) for quoting, booking, tendering, tracking, and managing freight shipments autonomously. Covers carriers, shippers, shipper accounts, load offers and bids, capacity, route duration, shipment documents and events, shipment scoring, and a full webhook surface (quote, shipment, load, bid, and carrier events). Authenticated with JWT tokens (RS256, RSA 4096) using Application-JWT or User-JWT security schemes; tokens should be short-lived (~1 minute) and supplied via the Authorization header.

- **Human URL:** [https://developer.loadsmart.com/docs/shipperguide/overview/getting-started](https://developer.loadsmart.com/docs/shipperguide/overview/getting-started)
- **Base URL:** `https://api.loadsmart.com`

#### Tags

- Freight
- Shipping
- Quotes
- Loads
- Bids
- Webhooks
- Carriers
- Shippers

#### Properties

- [Documentation](https://developer.loadsmart.com/docs/shipperguide/overview/getting-started)
- [API Reference](https://developer.loadsmart.com/docs/shipperguide/api-reference)
- [OpenAPI](openapi/loadsmart-shipperguide-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/loadsmart-shipperguide.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/loadsmart-shipperguide.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Open A P I Source](https://developer.loadsmart.com/api/openapi.yaml)
- [Webhooks](https://developer.loadsmart.com/docs/shipperguide/api-reference)
- [Sandbox](https://api.sandbox.loadsmart.com)
- [Authentication](https://developer.loadsmart.com/docs/shipperguide/overview/getting-started)
- [Postman](https://community.loadsmart.com/hc/en-us/articles/14945962355091-Importing-the-Postman-Collection) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)

### Opendock Nova (Neutron) API

Production REST API at https://neutron.opendock.com (staging neutron.staging.opendock.com) powering the Opendock Nova warehouse dock-scheduling platform. 151 endpoints covering warehouses, docks, loadtypes, appointments, carriers, users, organizations, custom-forms and custom-tags, gates, yards, hours of operation, ETAs, reports, billing, asset tracking, and integrations. Authenticated with JWT bearer tokens in the Authorization header; complementary Subspace WebSocket API streams Created/Updated/Deleted events for near-real-time integrations.

- **Human URL:** [https://developer.loadsmart.com/docs/opendock/overview/getting-started](https://developer.loadsmart.com/docs/opendock/overview/getting-started)
- **Base URL:** `https://neutron.opendock.com`

#### Tags

- Dock Scheduling
- Warehouse
- Appointments
- Yard Management
- Carriers
- Webhooks
- WebSockets

#### Properties

- [Documentation](https://developer.loadsmart.com/docs/opendock/overview/getting-started)
- [API Reference](https://developer.loadsmart.com/docs/opendock/category/overview)
- [OpenAPI](openapi/loadsmart-opendock-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/loadsmart-opendock.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/loadsmart-opendock.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Open A P I Source](https://neutron.opendock.com/docs-json)
- [Swagger U I](https://neutron.opendock.com/docs)
- [Web Sockets](https://developer.loadsmart.com/docs/opendock/overview/websockets)
- [Sandbox](https://neutron.staging.opendock.com)
- [Postman](https://www.postman.com/opendock/workspace/public-nova-workspace/) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Community](https://community.loadsmart.com/hc/en-us/sections/24987828169619-Opendock-Nova-Warehouse-API)

## Common Properties

- [Website](https://loadsmart.com)
- [Developer Portal](https://developer.loadsmart.com)
- [Documentation](https://developer.loadsmart.com/docs/)
- [API Reference](https://developer.loadsmart.com/docs/shipperguide/api-reference)
- [OpenAPI](https://developer.loadsmart.com/api/openapi.yaml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [About](https://loadsmart.com/about/)
- [Careers](https://loadsmart.com/careers/)
- [Contact](https://loadsmart.com/contact/)
- [Blog](https://blog.loadsmart.com/)
- [Community](https://community.loadsmart.com/)
- [Shipper Guide](https://loadsmart.com/shippers/shipperguide-tms/)
- [Managed Transportation](https://loadsmart.com/shippers/managed-transportation/)
- [Freight Intel A I](https://loadsmart.com/freightintel-ai/)
- [Private Fleet Optimizer](https://loadsmart.com/shippers/private-fleet-optimizer/)
- [Flatbed Messenger](https://loadsmart.com/flatbed-messenger/)
- [Carrier Loadboard](https://loadsmart.com/carriers/loadboard/)
- [Carrier Guide](https://loadsmart.com/carriers/carrierguide-tms/)
- [Factoring](https://loadsmart.com/carriers/factoring/)
- [Opendock](https://opendock.com/)
- [Nav Trac](https://loadsmart.com/warehouse/navtrac/)
- [Integrations](https://loadsmart.com/integrations/)
- [Oracle Integration](https://loadsmart.com/integrations/oracle/)
- [Mercury Gate Integration](https://loadsmart.com/integrations/mercury-gate/)
- [GitHub Organization](https://github.com/loadsmart)
- [Twitter](https://twitter.com/LoadSmartUS)
- [LinkedIn](https://www.linkedin.com/company/loadsmart)
- [YouTube](https://www.youtube.com/channel/UCN-pkKcoMargmyL0Br3-H5w)
- [Instagram](https://www.instagram.com/loadsmart)
- [Facebook](https://www.facebook.com/loadsmartUS)
- [Plans](plans/loadsmart-plans-pricing.yml)
- [Rate Limits](rate-limits/loadsmart-rate-limits.yml)
- [Fin Ops](finops/loadsmart-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
