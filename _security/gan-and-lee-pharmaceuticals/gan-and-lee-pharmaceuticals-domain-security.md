---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ganlee.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: ganlee.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gan And Lee Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gan & Lee Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gan & Lee Pharmaceuticals
provider_slug: gan-and-lee-pharmaceuticals
slug: gan-and-lee-pharmaceuticals-domain-security
source_filename: gan-and-lee-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ganlee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: ganlee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gan-and-lee-pharmaceuticals/refs/heads/main/security/gan-and-lee-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceuticals
- Diabetes
- Insulin
- Oncology
- Biotechnology
- Medical Devices
- Healthcare
- China
---
