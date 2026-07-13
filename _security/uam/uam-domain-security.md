---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uam.es
  spf: true
hosts:
- cert_expires: Dec 17 09:47:13 2026 GMT
  host: www.uam.es
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 09:47:13 2026 GMT
  host: repositorio.uam.es
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autonomous University of Madrid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Autonomous University of Madrid
provider_slug: uam
slug: uam-domain-security
source_filename: uam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uam.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 09:47:13 2026 GMT\n  hsts: false\n- host: repositorio.uam.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 09:47:13 2026 GMT\n  hsts: false\ndomains:\n- domain: uam.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uam/refs/heads/main/security/uam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Spain
- Open Access
- Institutional Repository
- DSpace
- OAI-PMH
- Research
---
