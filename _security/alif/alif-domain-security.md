---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alifsemi.com
  spf: true
hosts:
- cert_expires: Sep  5 05:14:43 2026 GMT
  host: alifsemi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alif, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alif
provider_slug: alif
slug: alif-domain-security
source_filename: alif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alifsemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:14:43 2026 GMT\n  hsts: false\ndomains:\n- domain: alifsemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alif/refs/heads/main/security/alif-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Hardtech
- Semiconductors
- Microcontrollers
- Edge AI
- Machine Learning
- Embedded
- IoT
- Generative AI
- MCU
---
