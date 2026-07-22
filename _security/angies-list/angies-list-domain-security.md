---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: angi.com
  spf: true
hosts:
- cert_expires: Oct  6 19:46:14 2026 GMT
  host: www.angi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angies List Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angie’s List, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Angie’s List
provider_slug: angies-list
slug: angies-list-domain-security
source_filename: angies-list-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.angi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:46:14 2026 GMT\n  hsts: false\ndomains:\n- domain: angi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angies-list/refs/heads/main/security/angies-list-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Home Services
- Marketplace
- Reviews
- Ratings
- Local Services
- Consumer
- Contractors
---
