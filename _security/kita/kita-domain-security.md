---
api_specs:
- filename: kita-capture-openapi.yml
  format: yaml
  label: Kita Capture API
  slug: capture
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-capture-openapi.yml
- filename: kita-underwriter-openapi.yml
  format: yaml
  label: Kita AI Underwriter API
  slug: underwriter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/openapi/kita-underwriter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kita.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usekita.com
  spf: true
hosts:
- cert_expires: Aug 24 22:35:38 2026 GMT
  host: www.kita.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 22:12:47 2026 GMT
  host: portal.usekita.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 05:13:06 2026 GMT
  host: underwriter.kita.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kita Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kita, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kita
provider_slug: kita
slug: kita-domain-security
source_filename: kita-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kita.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:35:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.usekita.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: underwriter.kita.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:13:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kita.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: usekita.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kita/refs/heads/main/security/kita-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Underwriting
- Credit Scoring
- Document Intelligence
- Document Extraction
- Fraud Detection
- Artificial Intelligence
- Computer Vision
- Emerging Markets
- Loan Origination
---
