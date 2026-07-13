---
api_specs:
- filename: kpmg-openapi.yml
  format: yaml
  label: KPMG Origins (IWTS)
  slug: kpmg-origins-iwts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpmg/refs/heads/main/openapi/kpmg-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kpmg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kpmgorigins.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: kpmg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 17:15:01 2026 GMT
  host: help.kpmgorigins.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: app.kpmgorigins.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kpmg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KPMG, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KPMG
provider_slug: kpmg
slug: kpmg-domain-security
source_filename: kpmg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kpmg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.kpmgorigins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:15:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.kpmgorigins.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kpmg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kpmgorigins.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kpmg/refs/heads/main/security/kpmg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consulting
- Audit
- Tax
- Legal
- Professional Services
- Big Four
- Advisory
- AI
- Trusted AI
- ESG
- Sustainability
- Risk
- Regulation
- Cybersecurity
- Strategy
- Technology
- Workforce
- Research
- Insights
- Industry Analysis
- Transformation
- Pillar Two
- Waste Tracking
---
