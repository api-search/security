---
api_specs:
- filename: mobileapi-openapi.yml
  format: yaml
  label: MobileAPI
  slug: mobileapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mobileapi.dev
  spf: true
hosts:
- cert_expires: Sep  5 08:12:11 2026 GMT
  host: mobileapi.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:12:11 2026 GMT
  host: api.mobileapi.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mobileapi Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MobileAPI.dev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MobileAPI.dev
provider_slug: mobileapi-dev
slug: mobileapi-dev-domain-security
source_filename: mobileapi-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobileapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:12:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mobileapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:12:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mobileapi.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/security/mobileapi-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data API
- Developer Tools
- Device Specifications
- Mobile Data
- Phone Specs
- REST API
- SaaS
---
