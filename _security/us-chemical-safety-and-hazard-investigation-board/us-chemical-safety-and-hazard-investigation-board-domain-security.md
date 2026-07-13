---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: csb.gov
  spf: true
hosts:
- cert_expires: Aug 21 16:03:46 2026 GMT
  host: www.csb.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Chemical Safety And Hazard Investigation Board Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Chemical Safety and Hazard Investigation Board, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: US Chemical Safety and Hazard Investigation Board
provider_slug: us-chemical-safety-and-hazard-investigation-board
slug: us-chemical-safety-and-hazard-investigation-board-domain-security
source_filename: us-chemical-safety-and-hazard-investigation-board-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.csb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: csb.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-chemical-safety-and-hazard-investigation-board/refs/heads/main/security/us-chemical-safety-and-hazard-investigation-board-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal Government
- Chemical Safety
- Incident Investigation
- Hazardous Materials
- Public Safety
- Environmental Safety
---
