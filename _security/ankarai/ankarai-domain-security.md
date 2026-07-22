---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ankar.ai
  spf: false
hosts:
- cert_expires: Oct 13 11:32:00 2026 GMT
  host: ankar.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ankarai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ankar.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ankar.ai
provider_slug: ankarai
slug: ankarai-domain-security
source_filename: ankarai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ankar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ankar.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ankarai/refs/heads/main/security/ankarai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Patents
- Intellectual Property
- Legal Tech
- Patent Drafting
- Patent Prosecution
- IP Management
---
