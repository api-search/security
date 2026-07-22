---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: newfront.com
  spf: true
hosts:
- cert_expires: Aug 23 08:23:55 2026 GMT
  host: www.newfront.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newfront Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newfront Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Newfront Insurance
provider_slug: newfront-insurance
slug: newfront-insurance-domain-security
source_filename: newfront-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newfront.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:23:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: newfront.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newfront-insurance/refs/heads/main/security/newfront-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Insurance
- Insurtech
- Insurance Brokerage
- Employee Benefits
- Risk Management
- Business Insurance
---
