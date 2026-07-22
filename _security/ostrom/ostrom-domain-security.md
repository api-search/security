---
api_specs:
- filename: ostrom-openapi-original.json
  format: json
  label: Ostrom API
  slug: ostrom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ostrom.de
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ostrom-api.io
  spf: false
hosts:
- cert_expires: Oct 15 10:16:22 2026 GMT
  host: ostrom.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: sandbox.ostrom-api.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: production.ostrom-api.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ostrom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ostrom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ostrom
provider_slug: ostrom
slug: ostrom-domain-security
source_filename: ostrom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ostrom.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.ostrom-api.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: production.ostrom-api.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ostrom.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ostrom-api.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/security/ostrom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Electricity
- Green Energy
- Smart Meter
- Dynamic Pricing
- Germany
- Sustainability
- Webhooks
- API
---
