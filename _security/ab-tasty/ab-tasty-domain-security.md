---
api_specs:
- filename: decision-api-openapi.yml
  format: yaml
  label: AB Tasty Decision API
  slug: ab-tasty-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/openapi/decision-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abtasty.com
  spf: true
hosts:
- cert_expires: Sep  9 19:52:06 2026 GMT
  host: www.abtasty.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: developers.abtasty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:32:17 2026 GMT
  host: docs.abtasty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ab Tasty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AB Tasty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AB Tasty
provider_slug: ab-tasty
slug: ab-tasty-domain-security
source_filename: ab-tasty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abtasty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:52:06 2026 GMT\n  hsts: null\n- host: developers.abtasty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.abtasty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:32:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abtasty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/security/ab-tasty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
---
