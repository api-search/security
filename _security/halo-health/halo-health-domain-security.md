---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: halomentalhealth.com
  spf: true
hosts:
- cert_expires: Oct 14 03:28:26 2026 GMT
  host: halomentalhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Halo Health
provider_slug: halo-health
slug: halo-health-domain-security
source_filename: halo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: halomentalhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:28:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: halomentalhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-health/refs/heads/main/security/halo-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mental Health
- Healthcare
- Urgent Care
- Psychiatry
- Telehealth
- Behavioral Health
---
