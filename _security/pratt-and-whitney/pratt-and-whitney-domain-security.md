---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prattwhitney.com
  spf: true
hosts:
- cert_expires: Oct  5 19:53:07 2026 GMT
  host: www.prattwhitney.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pratt And Whitney Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pratt & Whitney, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pratt & Whitney
provider_slug: pratt-and-whitney
slug: pratt-and-whitney-domain-security
source_filename: pratt-and-whitney-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prattwhitney.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:53:07 2026 GMT\n  hsts: null\ndomains:\n- domain: prattwhitney.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pratt-and-whitney/refs/heads/main/security/pratt-and-whitney-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aerospace
- Defense
- Aviation
- Manufacturing
- Engines
- MRO
- RTX
---
