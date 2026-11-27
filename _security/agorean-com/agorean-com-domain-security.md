---
api_specs:
- filename: agorean-com-openapi-generated.yml
  format: yaml
  label: Agorean API
  slug: agorean-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agorean-com/openapi/_ae-authored/agorean-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agorean.com
  spf: true
hosts:
- cert_expires: Dec  3 04:34:43 2026 GMT
  host: agorean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agorean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agorean, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agorean
provider_slug: agorean-com
slug: agorean-com-domain-security
source_filename: agorean-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agorean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 04:34:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agorean.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agorean-com/security/agorean-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketplace
- Reviews
- Payments
- Agents
---
