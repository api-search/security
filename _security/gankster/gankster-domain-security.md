---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gankster.gg
  spf: true
hosts:
- cert_expires: Oct  9 20:46:52 2026 GMT
  host: gankster.gg
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gankster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gankster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gankster
provider_slug: gankster
slug: gankster-domain-security
source_filename: gankster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gankster.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:46:52 2026 GMT\n  hsts: false\ndomains:\n- domain: gankster.gg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gankster/refs/heads/main/security/gankster-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Gaming
- Esports
- Social
- LFG
- Matchmaking
---
