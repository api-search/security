---
api_specs:
- filename: lightning-labs-openapi.json
  format: json
  label: Lightning Labs LND API
  slug: lightning-labs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightning-labs/refs/heads/main/openapi/lightning-labs-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lightning.engineering
  spf: true
hosts:
- cert_expires: Aug 31 06:52:25 2026 GMT
  host: lightning.engineering
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightning Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightning Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lightning Labs
provider_slug: lightning-labs
slug: lightning-labs-domain-security
source_filename: lightning-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightning.engineering\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:52:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightning.engineering\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightning-labs/refs/heads/main/security/lightning-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bitcoin
- Crypto
- Lightning Network
- Payments
---
