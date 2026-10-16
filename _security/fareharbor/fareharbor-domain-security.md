---
api_specs:
- filename: fareharbor-home-openapi.yml
  format: yaml
  label: FareHarbor Integration Center Home API
  slug: fareharbor-integration-center-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/openapi/_original/fareharbor-home-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fareharbor.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: fareharbor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fareharbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FareHarbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FareHarbor
provider_slug: fareharbor
slug: fareharbor-domain-security
source_filename: fareharbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fareharbor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fareharbor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fareharbor/refs/heads/main/security/fareharbor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Booking
- SaaS
- Tourism
- Software
---
