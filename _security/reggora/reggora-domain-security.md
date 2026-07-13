---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reggora.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: reggora.io
  spf: false
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.reggora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.reggora.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reggora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reggora, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reggora
provider_slug: reggora
slug: reggora-domain-security
source_filename: reggora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reggora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.reggora.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reggora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: reggora.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reggora/refs/heads/main/security/reggora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Appraisal Management
- Mortgage
- Lending
- Real Estate
- Valuation
- Loan Origination
- LOS Integration
- Fintech
---
