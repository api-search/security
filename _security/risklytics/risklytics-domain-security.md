---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: risklytics.ai
  spf: true
hosts:
- cert_expires: Sep  1 17:43:57 2026 GMT
  host: www.risklytics.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:54:07 2026 GMT
  host: platform.risklytics.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:30:55 2026 GMT
  host: api.risklytics.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Risklytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Risklytics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Risklytics
provider_slug: risklytics
slug: risklytics-domain-security
source_filename: risklytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.risklytics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.risklytics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:54:07 2026 GMT\n  hsts: null\n- host: api.risklytics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:30:55 2026 GMT\n  hsts: null\ndomains:\n- domain: risklytics.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/risklytics/refs/heads/main/security/risklytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Risk
- Wildfire
- Property
- Catastrophe
- Analytics
- Machine Learning
- Underwriting
---
