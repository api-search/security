---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: alterego.io
  spf: true
hosts:
- cert_expires: Aug 26 22:38:44 2026 GMT
  host: www.alterego.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alterego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alterego, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Alterego
provider_slug: alterego
slug: alterego-domain-security
source_filename: alterego-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alterego.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alterego.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterego/refs/heads/main/security/alterego-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Wearables
- Silent Speech
- Human-Computer Interaction
- Neural Interface
- Consumer Hardware
---
