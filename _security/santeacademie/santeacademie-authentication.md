---
api_key_in: []
api_specs:
- filename: santeacademie-article-api-openapi.yml
  format: yaml
  label: Santé Académie Article API
  slug: santeacademie-article-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-article-api-openapi.yml
- filename: santeacademie-customcatalog-api-openapi.yml
  format: yaml
  label: Santé Académie Custom Catalog API
  slug: santeacademie-customcatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-customcatalog-api-openapi.yml
- filename: santeacademie-faq-api-openapi.yml
  format: yaml
  label: Santé Académie Faq API
  slug: santeacademie-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-faq-api-openapi.yml
- filename: santeacademie-health-facility-api-openapi.yml
  format: yaml
  label: Santé Académie Health Facility API
  slug: santeacademie-health-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-health-facility-api-openapi.yml
- filename: santeacademie-job-api-openapi.yml
  format: yaml
  label: Santé Académie Job API
  slug: santeacademie-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-job-api-openapi.yml
- filename: santeacademie-jobspace-api-openapi.yml
  format: yaml
  label: Santé Académie Job Space API
  slug: santeacademie-jobspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-jobspace-api-openapi.yml
- filename: santeacademie-mediacategory-api-openapi.yml
  format: yaml
  label: Santé Académie Media Category API
  slug: santeacademie-mediacategory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-mediacategory-api-openapi.yml
- filename: santeacademie-pharmacy-api-openapi.yml
  format: yaml
  label: Santé Académie Pharmacy API
  slug: santeacademie-pharmacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-pharmacy-api-openapi.yml
- filename: santeacademie-resource-api-openapi.yml
  format: yaml
  label: Santé Académie Resource API
  slug: santeacademie-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-resource-api-openapi.yml
- filename: santeacademie-sitemap-api-openapi.yml
  format: yaml
  label: Santé Académie Sitemap API
  slug: santeacademie-sitemap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-sitemap-api-openapi.yml
- filename: santeacademie-testimonial-api-openapi.yml
  format: yaml
  label: Santé Académie Testimonial API
  slug: santeacademie-testimonial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-testimonial-api-openapi.yml
- filename: santeacademie-topic-api-openapi.yml
  format: yaml
  label: Santé Académie Topic API
  slug: santeacademie-topic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/openapi/santeacademie-topic-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Santeacademie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Santé Académie declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Santé Académie
provider_slug: santeacademie
scheme_count: 0
schemes: []
slug: santeacademie-authentication
source_filename: santeacademie-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: derived\nsource: >-\n  openapi/santeacademie-frontstage-openapi.json + openapi/santeacademie-connector-openapi.json + live anonymous\n  probes of frontstage/contentstudio/backstage/crossguard.santeacademie.com on 2026-08-17\nnote: >-\n  Ran 0-working/derive-authentication.py first; it wrote nothing because neither specification declares a single\n  securityScheme. That is not a thin spec — it is the finding. Both public APIs are genuinely open: they require no\n  credential and returned 200 to anonymous GETs. There is no documented auth page to upgrade this from, because\n  Santé Académie publishes no developer documentation of any kind.\nsummary:\n  schemes_declared: 0\n  public_apis_requiring_credentials: 0\n  oauth2: false\n  openid_connect: false\n  api_key: false\n  http_bearer: false\n  mutual_tls: false\n  posture: open-read-only\napis:\n- api: Santé Académie Frontstage API\n  spec: openapi/santeacademie-frontstage-openapi.json\n  security_schemes:\
  \ []\n  root_security: absent\n  effective: none\n  verified:\n    method: probed\n    url: https://frontstage.santeacademie.com/api/jobs\n    http_status: 200\n    sent_credentials: false\n    note: returned the live French profession list (MED/Médecin …) with no Authorization header\n- api: Santé Académie Connector API\n  spec: openapi/santeacademie-connector-openapi.json\n  security_schemes: []\n  root_security: absent\n  effective: none\n  verified:\n    method: probed\n    url: https://frontstage.santeacademie.com/connector/api/faq\n    http_status: 200\n    sent_credentials: false\n    note: returned live published FAQ records with no Authorization header\ngated_surfaces:\n  note: >-\n    Recorded for completeness — these are Santé Académie's internal services on the same domain. They are NOT part\n    of the public API surface and nothing in this repo is derived from them. They are listed so a reader can see\n    that the open posture above is a deliberate split between a public\
  \ catalog and gated back-office systems, not an\n    oversight across the whole estate.\n  surfaces:\n  - host: contentstudio.santeacademie.com\n    url: https://contentstudio.santeacademie.com/api/docs\n    http_status: 401\n    body: '{\"type\":\"...rfc2616#section-10\",\"title\":\"An error occurred\",\"detail\":\"Full authentication is required to access this resource.\"}'\n    wall: session login (302 from / to /login); robots.txt disallows everything\n  - host: backstage.santeacademie.com\n    url: https://backstage.santeacademie.com/api\n    http_status: 401\n    wall: session login (302 from / to /login)\n  - host: crossguard.santeacademie.com\n    url: https://crossguard.santeacademie.com/api\n    http_status: 404\n    wall: no API route exposed; / 302s to /login\naccount_auth:\n  note: >-\n    Learner sign-in is a first-party session login at https://play.santeacademie.com/. No OAuth authorization server,\n    no OpenID Connect discovery document and no SSO metadata is published\
  \ — /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server 404 on every host (see well-known/santeacademie-well-known.yml).\nrecommendations:\n- >-\n  Declare the open posture explicitly in the specifications. An empty securitySchemes reads to a generator as\n  \"unknown\", not \"public\"; an explicit `security: []` at the document root says \"no credential required\" and lets a\n  client library skip auth setup instead of guessing.\n- >-\n  If the catalog APIs are meant to be public, publish them: a base URL, a rate-limit statement and a terms-of-use\n  line are the difference between an internal endpoint anyone can find and an API a partner can build on. If they\n  are NOT meant to be public, they are currently readable by anyone, unauthenticated, from any network.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santeacademie/refs/heads/main/authentication/santeacademie-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Edtech
- healthcare-training
- continuing-education
- dpc
- e-learning
- france
- healthcare-professionals
- course-catalog
- lms
---
