---
api_specs:
- filename: laurel-time-openapi-original.json
  format: json
  label: Laurel Time Service API
  slug: time
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/openapi/laurel-time-openapi-original.json
- filename: laurel-identity-openapi-original.json
  format: json
  label: Laurel Identity Service API
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/openapi/laurel-identity-openapi-original.json
- filename: laurel-ingestion-openapi-original.json
  format: json
  label: Laurel Ingestion Service API
  slug: ingestion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/openapi/laurel-ingestion-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: laurel.ai
  spf: true
hosts:
- cert_expires: Oct  4 09:02:22 2026 GMT
  host: www.laurel.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laurel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laurel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Laurel
provider_slug: laurel
slug: laurel-domain-security
source_filename: laurel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laurel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: laurel.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laurel/refs/heads/main/security/laurel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Timekeeping
- Time Tracking
- Legal
- Legal Tech
- Accounting
- Professional Services
- Billing
- Practice Management
- Work Intelligence
- Analytics
---
