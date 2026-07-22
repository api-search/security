---
api_specs:
- filename: nomos-openapi-original.json
  format: json
  label: Nomos API
  slug: nomos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomos.energy
  spf: true
hosts:
- cert_expires: Oct  5 23:25:28 2026 GMT
  host: api.nomos.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nomos
provider_slug: nomos
slug: nomos-domain-security
source_filename: nomos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nomos.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:25:28 2026 GMT\n  hsts: false\ndomains:\n- domain: nomos.energy\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/security/nomos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Electricity
- Utilities
- Embedded Finance
- Dynamic Pricing
- Billing
- Metering
- Smart Meter
- Germany
- OAuth
- Webhooks
---
