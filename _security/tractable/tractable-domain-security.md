---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tractable.ai
  spf: true
hosts:
- cert_expires: Sep 10 17:07:37 2026 GMT
  host: tractable.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tractable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tractable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tractable
provider_slug: tractable
slug: tractable-domain-security
source_filename: tractable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tractable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 17:07:37 2026 GMT\n  hsts: false\ndomains:\n- domain: tractable.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tractable/refs/heads/main/security/tractable-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- InsurTech
- Claims
- Auto Insurance
- Property Insurance
- Computer Vision
- Deep Learning
- Artificial Intelligence
- Damage Assessment
- FNOL
- Subrogation
- Underwriting
- Vehicle Inspection
- Fleet Management
- Salvage
---
