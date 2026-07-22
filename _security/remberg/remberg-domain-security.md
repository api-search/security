---
api_specs:
- filename: remberg-assets-openapi.json
  format: json
  label: remberg Assets API
  slug: remberg-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-assets-openapi.json
- filename: remberg-work-orders-openapi.json
  format: json
  label: remberg Work Orders API
  slug: remberg-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-orders-openapi.json
- filename: remberg-work-requests-openapi.json
  format: json
  label: remberg Work Requests API
  slug: remberg-work-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-work-requests-openapi.json
- filename: remberg-tickets-openapi.json
  format: json
  label: remberg Tickets API
  slug: remberg-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-tickets-openapi.json
- filename: remberg-parts-openapi.json
  format: json
  label: remberg Parts API
  slug: remberg-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-parts-openapi.json
- filename: remberg-organizations-openapi.json
  format: json
  label: remberg Organizations API
  slug: remberg-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-organizations-openapi.json
- filename: remberg-contacts-openapi.json
  format: json
  label: remberg Contacts API
  slug: remberg-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-contacts-openapi.json
- filename: remberg-users-openapi.json
  format: json
  label: remberg Users API
  slug: remberg-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-users-openapi.json
- filename: remberg-files-openapi.json
  format: json
  label: remberg Files API
  slug: remberg-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-files-openapi.json
- filename: remberg-forms-openapi.json
  format: json
  label: remberg Forms API
  slug: remberg-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-forms-openapi.json
- filename: remberg-procedures-openapi.json
  format: json
  label: remberg Procedures API
  slug: remberg-procedures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-procedures-openapi.json
- filename: remberg-ai-openapi.json
  format: json
  label: remberg AI Copilot API
  slug: remberg-ai-copilot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/openapi/remberg-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: remberg.de
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: api.remberg.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remberg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Remberg
provider_slug: remberg
slug: remberg-domain-security
source_filename: remberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.remberg.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: remberg.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remberg/refs/heads/main/security/remberg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Maintenance
- Asset Management
- CMMS
- EAM
- Field Service
- Work Orders
- Industrial
- SaaS
- Germany
---
