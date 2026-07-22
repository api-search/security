---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datafr.ee
  spf: true
hosts:
- cert_expires: Oct  2 11:04:43 2026 GMT
  host: datafr.ee
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Binu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Binu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Binu
provider_slug: binu
slug: binu-domain-security
source_filename: binu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datafr.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:04:43 2026 GMT\n  hsts: false\ndomains:\n- domain: datafr.ee\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/binu/refs/heads/main/security/binu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Connectivity
- Mobile Data
- Reverse Billing
- Zero Rating
- Telecommunications
- Africa
- Data Sponsorship
- Digital Inclusion
---
