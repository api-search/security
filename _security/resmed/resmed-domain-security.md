---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: resmed.com
  spf: true
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.resmed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Resmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resmed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Resmed
provider_slug: resmed
slug: resmed-domain-security
source_filename: resmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.resmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: resmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resmed/refs/heads/main/security/resmed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Medical Devices
- Healthcare
- Sleep Apnea
- Respiratory Care
- Digital Health
- Connected Care
- Fortune 1000
---
