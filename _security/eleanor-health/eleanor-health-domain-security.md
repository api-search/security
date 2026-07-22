---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eleanorhealth.com
  spf: true
hosts:
- cert_expires: Oct  2 22:44:15 2026 GMT
  host: www.eleanorhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eleanor Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eleanor Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eleanor Health
provider_slug: eleanor-health
slug: eleanor-health-domain-security
source_filename: eleanor-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eleanorhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eleanorhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eleanor-health/refs/heads/main/security/eleanor-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Mental Health
- Addiction Treatment
- Substance Use Disorder
- Telehealth
- Value-Based Care
- Medication-Assisted Treatment
---
