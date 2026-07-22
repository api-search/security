---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: himaxwell.com
  spf: true
hosts:
- cert_expires: Aug 31 04:43:46 2026 GMT
  host: himaxwell.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maxwell Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maxwell Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Maxwell Financial
provider_slug: maxwell-financial
slug: maxwell-financial-domain-security
source_filename: maxwell-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: himaxwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:43:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: himaxwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxwell-financial/refs/heads/main/security/maxwell-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mortgage
- Lending
- Fintech
- Financial Services
- Loan Origination
- Mortgage Technology
---
