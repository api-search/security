---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: join9am.com
  spf: true
hosts:
- cert_expires: Aug 26 15:05:40 2026 GMT
  host: join9am.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 9Am Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 9am Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 9am Health
provider_slug: 9am-health
slug: 9am-health-domain-security
source_filename: 9am-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: join9am.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 15:05:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: join9am.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/9am-health/refs/heads/main/security/9am-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Telehealth
- Digital Health
- Diabetes
- Metabolic Health
- Weight Loss
- Pharmacy
- Chronic Care
---
