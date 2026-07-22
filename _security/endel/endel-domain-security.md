---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: endel.io
  spf: true
hosts:
- cert_expires: Jan 18 23:59:59 2027 GMT
  host: endel.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Endel
provider_slug: endel
slug: endel-domain-security
source_filename: endel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: endel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endel/refs/heads/main/security/endel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wellness
- Audio
- Soundscapes
- Music
- Sleep
- Focus
- Consumer App
---
