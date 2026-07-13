---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dnfsb.gov
  spf: true
hosts:
- cert_expires: Sep 12 15:41:51 2026 GMT
  host: www.dnfsb.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defense Nuclear Facilities Safety Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defense Nuclear Facilities Safety Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Defense Nuclear Facilities Safety Board
provider_slug: defense-nuclear-facilities-safety-board
slug: defense-nuclear-facilities-safety-board-domain-security
source_filename: defense-nuclear-facilities-safety-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnfsb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:41:51 2026 GMT\n  hsts: null\ndomains:\n- domain: dnfsb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defense-nuclear-facilities-safety-board/refs/heads/main/security/defense-nuclear-facilities-safety-board-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Defense
- DNFSB
- Energy
- Federal Government
- Health
- Independent Agency
- Nuclear
- Safety
---
