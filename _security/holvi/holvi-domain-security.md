---
api_specs:
- filename: holvi-psd2-openapi.yml
  format: yaml
  label: Holvi PSD2 API
  slug: holvi-psd2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holvi/refs/heads/main/openapi/holvi-psd2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: holvi.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: holvi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holvi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holvi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Holvi
provider_slug: holvi
slug: holvi-domain-security
source_filename: holvi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: holvi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: holvi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holvi/refs/heads/main/security/holvi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Fintech
- Payments
- Business Banking
- PSD2
- Open Banking
- SEPA
- Finland
---
