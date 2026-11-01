---
api_specs:
- filename: duve-openapi-generated.yml
  format: yaml
  label: Duve API
  slug: duve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duve/openapi/_ae-authored/duve-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: duve.com
  spf: true
hosts:
- cert_expires: Dec 18 07:35:09 2026 GMT
  host: duve.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Duve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Duve
provider_slug: duve
slug: duve-domain-security
source_filename: duve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 07:35:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: duve.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/duve/security/duve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- GuestExperience
- SaaS
- AI
- RevenueOptimization
- Company
---
