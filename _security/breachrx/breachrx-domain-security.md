---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: breachrx.com
  spf: true
hosts:
- cert_expires: Dec 18 08:35:42 2026 GMT
  host: www.breachrx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Breachrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BreachRx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BreachRx
provider_slug: breachrx
slug: breachrx-domain-security
source_filename: breachrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breachrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 08:35:42 2026 GMT\n  hsts: null\ndomains:\n- domain: breachrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breachrx/refs/heads/main/security/breachrx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cybersecurity
- Incident Response
- Platform
- AI
- Regulatory Intelligence
---
