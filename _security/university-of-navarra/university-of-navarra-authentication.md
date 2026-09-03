---
api_key_in: []
api_specs:
- filename: university-of-navarra-revistas-oai-pmh-openapi.yml
  format: yaml
  label: Revistas Cientificas OAI-PMH (Servicio de Publicaciones)
  slug: revistas-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-navarra/refs/heads/main/openapi/university-of-navarra-revistas-oai-pmh-openapi.yml
auth_types: []
description: How the University of Navarra's verified machine-readable surfaces authenticate callers. Probed 2026-09-01; nothing here is inferred from documentation.
kind: authentication
layout: security
method: probed
name: University Of Navarra Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Navarra declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Navarra
provider_slug: university-of-navarra
scheme_count: 0
schemes: []
slug: university-of-navarra-authentication
source_filename: university-of-navarra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Navarra — Authentication\ndescription: >-\n  How the University of Navarra's verified machine-readable surfaces authenticate\n  callers. Probed 2026-09-01; nothing here is inferred from documentation.\ngenerated: '2026-09-01'\nmethod: probed\nsource:\n  - https://revistas.unav.edu/index.php/index/oai?verb=Identify\n  - https://revistas.unav.edu/index.php/anuario-de-historia-iglesia/api/v1/issues\n  - https://dadun.unav.edu/dspace-oai/request?verb=Identify\n  - https://unika.unav.edu/primaws/rest/pub/pnxs\nsurfaces:\n  - surface: Revistas Cientificas OAI-PMH\n    url: https://revistas.unav.edu/index.php/index/oai\n    operator: institution\n    auth: none\n    status: 200\n    detail: >-\n      Open, unauthenticated OAI-PMH 2.0 harvesting interface. No API key, no\n      registration, no rate-limit headers observed. Protocol errors are returned\n      as HTTP 200 with an OAI <error> element rather than an HTTP status.\n  - surface: Revistas Cientificas\
  \ OJS REST API\n    url: https://revistas.unav.edu/index.php/{journal}/api/v1/issues\n    operator: institution\n    auth: api_key\n    status: 403\n    detail: >-\n      The OJS 3.4 REST API is deployed but closed: /api/v1/issues,\n      /api/v1/submissions and /api/v1/contexts all return 403 application/json to\n      an anonymous caller. OJS gates these behind a per-user API token issued from\n      the journal admin interface; no public self-service issuance was found.\n  - surface: DADUN institutional repository\n    url: https://dadun.unav.edu/dspace-oai/request\n    operator: tenant\n    auth: unknown\n    status: 403\n    detail: >-\n      Every path on dadun.unav.edu and dadun.unav.es returns 403 to automated\n      clients, including with a desktop browser User-Agent — an Anubis-style bot\n      challenge in front of the whole host, not an authentication requirement on\n      the API. The underlying OAI-PMH interface is registered publicly in ROAR,\n      Hispana and REBIUN.\n\
  \  - surface: Unika library discovery (Ex Libris Primo VE)\n    url: https://unika.unav.edu/primaws/rest/pub/pnxs\n    operator: tenant\n    auth: none\n    status: 200\n    detail: >-\n      Ex Libris Primo VE's public \"primaws\" search API answers unauthenticated\n      JSON requests for view id 34UNAV_INST:VU1. The contract is Ex Libris's; the\n      tenancy and the catalog data are the university's.\n  - surface: Institutional SAML Identity Provider\n    url: https://www.rediris.es/sir/unavidp\n    operator: federation\n    auth: saml2\n    detail: >-\n      SAML 2.0 Web SSO. Trust is established through RedIRIS SIR2 metadata and\n      eduGAIN interfederation rather than per-client credentials. Scope unav.es,\n      REFEDS Sirtfi declared.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-navarra/refs/heads/main/authentication/university-of-navarra-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Spain
- Private Research University
- Open Access
- Institutional Repository
- Scholarly Publishing
- OAI-PMH
- Identity Federation
- Library
---
