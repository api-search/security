---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: virtualtechfrontier.com
  spf: true
hosts:
- cert_expires: Sep 13 21:59:39 2026 GMT
  host: virtualtechfrontier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virtualtech Frontier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtualtech Frontier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Virtualtech Frontier
provider_slug: virtualtech-frontier
slug: virtualtech-frontier-domain-security
source_filename: virtualtech-frontier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtualtechfrontier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virtualtechfrontier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtualtech-frontier/refs/heads/main/security/virtualtech-frontier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Metaverse
- Extended Reality
- Immersive Technology
- Virtual Worlds
- Experiential Events
- Artificial Intelligence
---
