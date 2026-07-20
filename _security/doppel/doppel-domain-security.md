---
api_specs:
- filename: doppel-openapi-original.yml
  format: yaml
  label: Doppel API
  slug: doppel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: doppel.com
  spf: true
hosts:
- cert_expires: Aug 22 12:41:28 2026 GMT
  host: www.doppel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 12:41:28 2026 GMT
  host: api.doppel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doppel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doppel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Doppel
provider_slug: doppel
slug: doppel-domain-security
source_filename: doppel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doppel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:41:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.doppel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:41:28 2026 GMT\n  hsts: null\ndomains:\n- domain: doppel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/security/doppel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Digital Risk Protection
- Social Engineering Defense
- Brand Protection
- Anti-Phishing
- Threat Intelligence
- Human Risk Management
- Takedowns
---
