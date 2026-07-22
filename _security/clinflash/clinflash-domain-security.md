---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: clinflash.com
  spf: true
hosts:
- cert_expires: Jan 28 01:10:33 2027 GMT
  host: www.clinflash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clinflash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clinflash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Clinflash
provider_slug: clinflash
slug: clinflash-domain-security
source_filename: clinflash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clinflash.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 01:10:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clinflash.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clinflash/refs/heads/main/security/clinflash-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Company
- Clinical Trials
- Clinical Research
- Healthcare
- Life Sciences
- EDC
- Pharmacovigilance
- SaaS
- Pharmaceutical
---
