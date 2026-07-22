---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pop.in
  spf: true
hosts:
- cert_expires: Oct 15 15:48:24 2026 GMT
  host: pop.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Popin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pop.in, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pop.in
provider_slug: popin
slug: popin-domain-security
source_filename: popin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pop.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:48:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pop.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popin/refs/heads/main/security/popin-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Social
- Gaming
- Multiplayer
- Mobile
- Consumer
- Entertainment
---
