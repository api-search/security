---
api_specs:
- filename: telus-insights-location-api.postman_collection.json
  format: json
  label: TELUS Insights Location API
  slug: telus-insights-location-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/telus/refs/heads/main/collections/telus-insights-location-api.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telus.com
  spf: true
hosts:
- cert_expires: Sep 24 10:42:38 2026 GMT
  host: www.telus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 14:44:07 2026 GMT
  host: docs.insights.telus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 17:17:43 2026 GMT
  host: location-api.insights.telus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TELUS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TELUS
provider_slug: telus
slug: telus-domain-security
source_filename: telus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:42:38 2026 GMT\n  hsts: null\n- host: docs.insights.telus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:44:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: location-api.insights.telus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 17:17:43 2026 GMT\n  hsts: null\ndomains:\n- domain: telus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telus/refs/heads/main/security/telus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Canada
- Mobile Network Operator
- Broadband
- Network APIs
- CAMARA
- Open Gateway
- SIM Swap
- Identity Verification
- Location Intelligence
- IoT
- 5G
- Healthcare
- Electronic Medical Records
- GraphQL
- Webhooks
- Geospatial
---
