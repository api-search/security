---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iconicgames.io
  spf: true
hosts:
- cert_expires: Sep  5 20:39:26 2026 GMT
  host: iconicgames.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iconic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iconic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Iconic
provider_slug: iconic
slug: iconic-domain-security
source_filename: iconic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iconicgames.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:39:26 2026 GMT\n  hsts: false\ndomains:\n- domain: iconicgames.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iconic/refs/heads/main/security/iconic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Gaming
- Interactive Storytelling
- Generative AI
- Machine Learning
- Video Games
- Conversational AI
---
