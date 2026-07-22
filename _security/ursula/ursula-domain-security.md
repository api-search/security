---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ursula.ai
  spf: true
hosts:
- cert_expires: Oct  8 11:08:10 2026 GMT
  host: ursula.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ursula Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ursula, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ursula
provider_slug: ursula
slug: ursula-domain-security
source_filename: ursula-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ursula.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:08:10 2026 GMT\n  hsts: null\ndomains:\n- domain: ursula.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ursula/refs/heads/main/security/ursula-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- AI Characters
- Gaming
- LLM
- Brazil
---
