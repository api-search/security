---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: microsec.io
  spf: true
hosts:
- cert_expires: Jan  7 05:46:02 2027 GMT
  host: www.microsec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Microsec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Microsec
provider_slug: microsec
slug: microsec-domain-security
source_filename: microsec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 05:46:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsec.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/microsec/security/microsec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- IoT
- OT
- Cloud
---
