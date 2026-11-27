---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: votervoice.net
  spf: true
hosts:
- cert_expires: Feb  7 21:33:44 2027 GMT
  host: votervoice.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Votervoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Votervoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Votervoice
provider_slug: votervoice
slug: votervoice-domain-security
source_filename: votervoice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: votervoice.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 21:33:44 2027 GMT\n  hsts: false\ndomains:\n- domain: votervoice.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/votervoice/security/votervoice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advocacy
- Grassroots
- Digital Advocacy
- Advertising Services
- Election Hub
- ROI Reporting
---
