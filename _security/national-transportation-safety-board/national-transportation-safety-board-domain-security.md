---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ntsb.gov
  spf: true
hosts:
- cert_expires: Sep  4 06:15:17 2026 GMT
  host: www.ntsb.gov
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Transportation Safety Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Transportation Safety Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Transportation Safety Board
provider_slug: national-transportation-safety-board
slug: national-transportation-safety-board-domain-security
source_filename: national-transportation-safety-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ntsb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 06:15:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ntsb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-transportation-safety-board/refs/heads/main/security/national-transportation-safety-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Safety
- Transportation
---
