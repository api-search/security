---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sensely.com
  spf: false
hosts:
- cert_expires: Nov 10 00:04:34 2026 GMT
  host: sensely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: apis.sensely.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sensely, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Sensely
provider_slug: sensely
slug: sensely-domain-security
source_filename: sensely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sensely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 00:04:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.sensely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sensely.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensely/refs/heads/main/security/sensely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Conversational AI
- Virtual Assistant
- Symptom Checker
- Patient Engagement
- Health Insurance
- Mental Health
- SDK
---
