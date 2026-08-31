---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mantrahealth.com
  spf: true
hosts:
- cert_expires: Oct  1 23:01:43 2026 GMT
  host: mantrahealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:52:19 2026 GMT
  host: api.mantrahealth.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mantra Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mantra Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mantra Health
provider_slug: mantra-health
slug: mantra-health-domain-security
source_filename: mantra-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mantrahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mantrahealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:52:19 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: mantrahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mantra-health/refs/heads/main/security/mantra-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Telehealth
- Higher Education
- Digital Health
- Patient Engagement
- HIPAA
- GraphQL
---
