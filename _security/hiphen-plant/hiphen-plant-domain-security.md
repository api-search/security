---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hiphen-plant.com
  spf: true
hosts:
- cert_expires: Oct  2 23:14:45 2026 GMT
  host: www.hiphen-plant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hiphen Plant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hiphen Plant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hiphen Plant
provider_slug: hiphen-plant
slug: hiphen-plant-domain-security
source_filename: hiphen-plant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hiphen-plant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:14:45 2026 GMT\n  hsts: false\ndomains:\n- domain: hiphen-plant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiphen-plant/refs/heads/main/security/hiphen-plant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- Image Analytics
- Plant Science
- Research
---
