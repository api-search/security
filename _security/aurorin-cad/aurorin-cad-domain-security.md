---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aurorincad.com
  spf: true
hosts:
- cert_expires: Oct  9 22:35:30 2026 GMT
  host: www.aurorincad.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aurorin Cad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurorin CAD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aurorin CAD
provider_slug: aurorin-cad
slug: aurorin-cad-domain-security
source_filename: aurorin-cad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aurorincad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 22:35:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aurorincad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurorin-cad/refs/heads/main/security/aurorin-cad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CAD
- Mechanical Engineering
- Product Design
- Artificial Intelligence
- Hardware
- Manufacturing
- Desktop Software
- Y Combinator
---
