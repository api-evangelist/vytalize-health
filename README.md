# Vytalize Health

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

Vytalize Health is a Medicare Accountable Care Organization (ACO) and value-based care company based
in Hoboken, New Jersey. It partners with independent primary care practices, group practices,
community health centers and existing ACOs, pairing shared-savings economics with a technology and
clinical services stack: **Vytal Insights** (clinical decision support built on claims, clinical
notes, hospital ADT feeds and social determinants data), **Vytal Care** (remote and in-home care
programs) and **Vytal Network** (specialist and hospital network management).

## API surface

**Vytalize Health publishes no public API.** Contract discovery was run in full on 2026-09-04 and
found nothing to catalog:

- No developer portal, documentation host or API reference. The site's own `page-sitemap.xml` lists
  24 pages and none of them is developer-facing; `developer.`, `developers.`, `docs.`, `api.`,
  `portal.` and `status.` subdomains do not resolve.
- No OpenAPI, Swagger, GraphQL SDL, AsyncAPI, WSDL, protobuf or OGC contract on any host.
- No `llms.txt`, no `/apis.json`, no MCP server, no A2A agent card, and no document on any probed
  `/.well-known/` path on any host — see `well-known/`.
- No first-party SDK on npm, PyPI, RubyGems or Packagist. The public GitHub organization
  [vytalizehealth](https://github.com/vytalizehealth) holds one repository, a fork of a third-party
  PHP library.

Two API-adjacent surfaces *do* exist and are recorded for what they are:

1. **`prod-banzai-services.vytalizehealth.com`** — the product backend the partner portal calls,
   discovered by reading the portal's own public JavaScript bundle. It is an AWS load balancer whose
   port 443 times out from the public internet on every published address, so it is network-gated
   rather than merely undocumented.
2. **`www.vytalizehealth.com/wp-json/`** — the marketing site's WordPress REST API, open and serving
   513 routes. It is content-management infrastructure, not a Vytalize product API, and is
   deliberately **not** registered as an API in `apis.yml`.

Artifacts in this repository therefore record measured absence — which registries were searched,
which paths were probed, and what each returned — rather than a contract.

## Source

- Company site: https://www.vytalizehealth.com/
- Partner portal: https://app.vytalizehealth.com/
- Secondary-market listing that surfaced the company: https://forgeglobal.com/vytalize-health_stock/
