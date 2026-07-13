---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: legiscan.com
  spf: true
hosts:
- cert_expires: Sep 19 22:42:56 2026 GMT
  host: legiscan.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 10:50:11 2026 GMT
  host: api.legiscan.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Legiscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LegiScan, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LegiScan
provider_slug: legiscan
slug: legiscan-domain-security
source_filename: legiscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: legiscan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:42:56 2026 GMT\n  hsts: null\n- host: api.legiscan.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 10:50:11 2026 GMT\n  hsts: null\ndomains:\n- domain: legiscan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legiscan/refs/heads/main/security/legiscan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Legislative Tracking
- Government
- Bills
- Voting Records
- State Legislation
- Congressional Data
- Civic Tech
---
