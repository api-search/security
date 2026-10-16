---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: standab.com
  spf: false
hosts:
- cert_expires: Jan  2 02:09:57 2027 GMT
  host: standab.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Standab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Standab
provider_slug: standab
slug: standab-domain-security
source_filename: standab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 02:09:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: standab.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standab/refs/heads/main/security/standab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Micromobility
- Infrastructure
- Parking
- Charging
---
