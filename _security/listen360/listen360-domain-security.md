---
api_specs:
- filename: listen360-openapi-generated.yml
  format: yaml
  label: Listen360 API
  slug: listen360-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listen360/openapi/_ae-authored/listen360-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: listen360.com
  spf: true
hosts:
- cert_expires: Feb  7 17:50:21 2027 GMT
  host: listen360.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Listen360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listen360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Listen360
provider_slug: listen360
slug: listen360-domain-security
source_filename: listen360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: listen360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 17:50:21 2027 GMT\n  hsts: false\ndomains:\n- domain: listen360.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/listen360/security/listen360-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Customer Experience
- Feedback Management
- Reputation Management
- Enterprise Software
- Multi-Location Brands
- NPS
- Survey Platform
---
