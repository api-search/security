---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: indigov.com
  spf: true
hosts:
- cert_expires: Oct  8 03:10:34 2026 GMT
  host: indigov.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indigov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indigov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Indigov
provider_slug: indigov
slug: indigov-domain-security
source_filename: indigov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indigov.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:10:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: indigov.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indigov/refs/heads/main/security/indigov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- GovTech
- Constituent Relationship Management
- CRM
- Civic Technology
- Casework
- Constituent Communications
- Customer Data Platform
- Public Sector
---
