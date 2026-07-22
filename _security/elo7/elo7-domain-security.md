---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elo7.com.br
  spf: true
hosts:
- cert_expires: Sep 26 01:43:30 2026 GMT
  host: www.elo7.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elo7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elo7, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: elo7
provider_slug: elo7
slug: elo7-domain-security
source_filename: elo7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elo7.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:43:30 2026 GMT\n  hsts: null\ndomains:\n- domain: elo7.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elo7/refs/heads/main/security/elo7-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- E-commerce
- Handmade
- Crafts
- Brazil
- Consumer
- Defunct
---
