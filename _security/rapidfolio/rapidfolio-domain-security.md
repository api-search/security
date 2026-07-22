---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rapidfolio.com
  spf: true
hosts:
- cert_expires: Oct  4 20:24:22 2026 GMT
  host: rapidfolio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 09:03:09 2026 GMT
  host: docs.rapidfolio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapidfolio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rapidfolio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rapidfolio
provider_slug: rapidfolio
slug: rapidfolio-domain-security
source_filename: rapidfolio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapidfolio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rapidfolio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 09:03:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rapidfolio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidfolio/refs/heads/main/security/rapidfolio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Workflow Automation
- Artificial Intelligence
- Agents
- Compliance
- KYC
- Fraud
- Back Office
---
