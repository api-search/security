---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oxaide.com
  spf: true
hosts:
- cert_expires: Jan 24 18:39:51 2027 GMT
  host: oxaide.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oxaide Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oxaide Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oxaide Research
provider_slug: oxaide-com
slug: oxaide-com-domain-security
source_filename: oxaide-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oxaide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 18:39:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oxaide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/oxaide-com/security/oxaide-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company Verification
- Singapore registers
- Transport data
- Guides
- AI Desk
---
