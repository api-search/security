---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keepe.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: keepe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.keepe.com
  hsts: null
  https: true
  note: private application backend (nginx/ELB, Express); no public spec or docs
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Keepe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keepe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Keepe
provider_slug: keepe
slug: keepe-domain-security
source_filename: keepe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keepe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.keepe.com\n  https: true\n  tls_version: TLSv1.2\n  hsts: null\n  note: private application backend (nginx/ELB, Express); no public spec or docs\ndomains:\n- domain: keepe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keepe/refs/heads/main/security/keepe-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Home Services
- Field Service
- Property Management
- HVAC
- Plumbing
- Electrical
- Marketplace
- Techstars
---
