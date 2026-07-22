---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sinovision-tech.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: sinovision-tech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sinovision Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sinovision-tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: sinovision-tech
provider_slug: sinovision-tech
slug: sinovision-tech-domain-security
source_filename: sinovision-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sinovision-tech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sinovision-tech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinovision-tech/refs/heads/main/security/sinovision-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Imaging
- Healthcare
- CT Scanner
- Medical Devices
- Radiology
- Artificial Intelligence
- Cloud Imaging
---
