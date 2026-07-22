---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: distance.tech
  spf: true
hosts:
- cert_expires: Oct 11 09:06:19 2026 GMT
  host: distance.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Distance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Distance
provider_slug: distance
slug: distance-domain-security
source_filename: distance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distance.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:06:19 2026 GMT\n  hsts: false\ndomains:\n- domain: distance.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distance/refs/heads/main/security/distance-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Frontier Tech
- Extended Reality
- Augmented Reality
- Computational Optics
- Lightfield
- Heads-Up Display
- Defense
- Automotive
- Aerospace
---
