---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arondite.com
  spf: true
hosts:
- cert_expires: Oct 14 18:29:14 2026 GMT
  host: arondite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arondite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arondite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arondite
provider_slug: arondite
slug: arondite-domain-security
source_filename: arondite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arondite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:29:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arondite.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arondite/refs/heads/main/security/arondite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai Ml
- Defense
- Defence Technology
- Military
- Situational Awareness
- Mission Orchestration
- Decision Support
---
