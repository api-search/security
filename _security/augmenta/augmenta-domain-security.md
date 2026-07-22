---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: augmenta.ai
  spf: true
hosts:
- cert_expires: Sep 30 13:28:00 2026 GMT
  host: www.augmenta.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augmenta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmenta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Augmenta
provider_slug: augmenta
slug: augmenta-domain-security
source_filename: augmenta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.augmenta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: augmenta.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmenta/refs/heads/main/security/augmenta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction
- AEC
- MEP
- Electrical Design
- Building Design
- BIM
- Revit
- Spatial AI
- Generative AI
- Foundation Models
- Generative Design
- Computational Geometry
- Optimization
- Data Centers
- Prefabrication
---
