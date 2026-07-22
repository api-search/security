---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: talkspace.com
  spf: true
hosts:
- cert_expires: Aug 14 02:59:23 2026 GMT
  host: www.talkspace.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talkspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Talkspace
provider_slug: talkspace
slug: talkspace-domain-security
source_filename: talkspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talkspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:59:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: talkspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkspace/refs/heads/main/security/talkspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Behavioral Health
- Mental Health
- Online Therapy
- Telehealth
- Psychiatry
- Medication Management
- Teen Therapy
- Couples Therapy
- Employee Assistance
- Health Insurance
- HIPAA
- Public Company
---
