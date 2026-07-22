---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: awarehealth.io
  spf: true
hosts:
- cert_expires: Sep  3 09:00:52 2026 GMT
  host: awarehealth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aware Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aware Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aware Health
provider_slug: aware-health
slug: aware-health-domain-security
source_filename: aware-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: awarehealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:00:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: awarehealth.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aware-health/refs/heads/main/security/aware-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Musculoskeletal
- MSK Care
- Virtual Care
- Telehealth
- Artificial Intelligence
- Employee Benefits
---
