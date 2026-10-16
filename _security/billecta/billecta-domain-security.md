---
api_specs:
- filename: billecta-openapi-generated.yml
  format: yaml
  label: Billecta API
  slug: billecta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/openapi/_ae-authored/billecta-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: billecta.com
  spf: true
hosts:
- cert_expires: Nov 23 13:39:51 2026 GMT
  host: billecta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billecta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billecta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Billecta
provider_slug: billecta
slug: billecta-domain-security
source_filename: billecta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billecta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 13:39:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billecta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billecta/refs/heads/main/security/billecta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- Invoicing
- Payments
- SaaS
- Sweden
- BusinessAutomation
---
