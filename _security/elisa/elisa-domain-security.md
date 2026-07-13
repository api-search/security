---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elisa.tech
  spf: true
hosts:
- cert_expires: Sep  6 18:54:28 2026 GMT
  host: elisa.tech
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elisa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELISA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ELISA
provider_slug: elisa
slug: elisa-domain-security
source_filename: elisa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elisa.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: elisa.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/security/elisa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded
- Linux
- Linux Foundation
- Safety
---
