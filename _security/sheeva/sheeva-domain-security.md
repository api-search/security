---
api_specs:
- filename: sheeva-openapi.yml
  format: yaml
  label: SheevaConnect API
  slug: sheevaconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/openapi/sheeva-openapi.yml
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sheeva.ai
  spf: true
hosts:
- cert_expires: Oct  1 17:48:05 2026 GMT
  host: sheeva.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: us-apis.sheeva.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: in-apis.sheeva.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Sheeva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sheeva, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sheeva
provider_slug: sheeva
slug: sheeva-domain-security
source_filename: sheeva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sheeva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:48:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us-apis.sheeva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\n- host: in-apis.sheeva.ai\n  https: false\ndomains:\n- domain: sheeva.ai\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheeva/refs/heads/main/security/sheeva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Connected Vehicles
- Automotive
- Payments
- Fintech
- In-Vehicle Payments
- EV Charging
- Parking
- Location Intelligence
- Mobility
---
