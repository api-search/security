---
api_specs:
- filename: evervault-openapi-original.json
  format: json
  label: Evervault API
  slug: evervault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/openapi/evervault-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: evervault.com
  spf: true
hosts:
- cert_expires: Sep 25 14:56:16 2026 GMT
  host: evervault.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evervault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evervault, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Evervault
provider_slug: evervault
slug: evervault-domain-security
source_filename: evervault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evervault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:56:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evervault.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evervault/refs/heads/main/security/evervault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Security
- Encryption
- Payments
- PCI Compliance
- Tokenization
- Cards
- Developer Tools
---
