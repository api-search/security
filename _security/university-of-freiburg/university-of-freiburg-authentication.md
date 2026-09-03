---
api_key_in: []
api_specs:
- filename: university-of-freiburg-freidok-plus-json-api-openapi.yml
  format: yaml
  label: FreiDok plus JSON API
  slug: freidok-json
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-freiburg/refs/heads/main/openapi/university-of-freiburg-freidok-plus-json-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Freiburg Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Freiburg declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Freiburg
provider_slug: university-of-freiburg
scheme_count: 0
schemes: []
slug: university-of-freiburg-authentication
source_filename: university-of-freiburg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Freiburg — authentication posture across public surfaces\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of each host listed below. No credentials of any kind were used or\n  attempted; every result is what an anonymous public client receives.\nsurfaces:\n  - surface: FreiDok plus JSON API\n    url: https://freidok.uni-freiburg.de/jsonApi/v1/publications\n    x-operator: institution\n    auth: none\n    evidence: 'GET without any header returned HTTP 200 and 267,771 records (numFound).'\n    notes: No API key, no registration, no quota documented, no auth-related response headers.\n  - surface: FreiDok plus OAI-PMH\n    url: https://freidok.uni-freiburg.de/oai/oai2.php?verb=Identify\n    x-operator: institution\n    auth: none\n    evidence: 'GET returned HTTP 200 OAI-PMH 2.0 Identify response.'\n  - surface: FreiData REST API (InvenioRDM deployment)\n    url: https://freidata.uni-freiburg.de/api/records\n    x-operator:\
  \ institution\n    auth: none for read\n    evidence: 'GET ?size=1 returned HTTP 200 with record hits, DOIs and file links.'\n    notes: >-\n      Write operations in InvenioRDM require a token; no token issuance process was found on the\n      public surface, so writing is treated as not publicly available.\n  - surface: University of Freiburg GitLab REST API v4\n    url: https://gitlab.uni-freiburg.de/api/v4/projects\n    x-operator: institution\n    auth: none for public projects; token required otherwise\n    evidence: >-\n      GET returned HTTP 200 listing 56 public projects (x-total: 56) with rate-limit headers\n      ratelimit-limit 60 / ratelimit-name throttle_unauthenticated_api. GET /api/v4/metadata\n      returned HTTP 401 {\"message\":\"401 Unauthorized\"}.\n  - surface: Uni-Freiburg Services status page API\n    url: https://status.uni-freiburg.de/api/status-page/ufr-services\n    x-operator: institution\n    auth: none\n    evidence: 'GET returned HTTP 200 application/json\
  \ config + monitor list; /metrics returned 401.'\n  - surface: myLogin Shibboleth Identity Provider (SAML 2.0)\n    url: https://mylogin.uni-freiburg.de/idp/shibboleth\n    x-operator: federation\n    auth: 'metadata is public; the IdP itself authenticates university accounts'\n    evidence: >-\n      GET returned HTTP 200 application/xml SAML 2.0 EntityDescriptor,\n      entityID https://mylogin.uni-freiburg.de/shibboleth,\n      OrganizationDisplayName \"Albert-Ludwigs-Universität Freiburg\".\n  - surface: Katalog plus library discovery\n    url: https://katalog.ub.uni-freiburg.de/\n    x-operator: institution\n    auth: not determinable\n    evidence: >-\n      HTTP 403 \"Access Denied — Der Zugang von Ihrer IP-Adresse ... aufgrund von Bot-Aktivitäten\n      ... gesperrt\". Live but blocked to our client; no conclusion drawn about any API behind it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-freiburg/refs/heads/main/authentication/university-of-freiburg-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Research
- Research Data
- Open Data
- Library
- Repository
- OAI-PMH
- Identity Federation
- Germany
---
