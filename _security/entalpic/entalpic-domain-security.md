---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: entalpic.ai
  spf: true
hosts:
- cert_expires: Oct  6 12:13:07 2026 GMT
  host: entalpic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entalpic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entalpic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Entalpic
provider_slug: entalpic
slug: entalpic-domain-security
source_filename: entalpic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entalpic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:13:07 2026 GMT\n  hsts: false\ndomains:\n- domain: entalpic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entalpic/refs/heads/main/security/entalpic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Materials Science
- Chemistry
- Simulation
- Deep Tech
- Semiconductors
- Batteries
- Catalysis
---
