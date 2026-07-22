---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azuria.com
  spf: true
hosts:
- cert_expires: Oct  6 15:21:51 2026 GMT
  host: azuria.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azuria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azuria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azuria
provider_slug: azuria
slug: azuria-domain-security
source_filename: azuria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azuria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:21:51 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: azuria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azuria/refs/heads/main/security/azuria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Water
- Infrastructure
- Utilities
- Pipeline Rehabilitation
- Construction
- Water Management
---
