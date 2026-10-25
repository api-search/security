---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evolutionmining.com.au
  spf: true
hosts:
- cert_expires: Nov 26 23:44:44 2026 GMT
  host: evolutionmining.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evolution Mining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evolution Mining, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Evolution Mining
provider_slug: evolution-mining
slug: evolution-mining-domain-security
source_filename: evolution-mining-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evolutionmining.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:44:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: evolutionmining.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolution-mining/refs/heads/main/security/evolution-mining-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Gold
- Copper
- Natural Resources
- Australia
- Canada
- ASX Listed
---
