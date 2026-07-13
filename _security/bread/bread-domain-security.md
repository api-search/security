---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: breadfinancial.com
  spf: true
hosts:
- cert_expires: Aug 26 21:51:58 2026 GMT
  host: www.breadfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developers.breadfinancial.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bread Financial, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bread Financial
provider_slug: bread
slug: bread-domain-security
source_filename: bread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.breadfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:51:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.breadfinancial.com\n  https: false\ndomains:\n- domain: breadfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bread/refs/heads/main/security/bread-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Buy Now Pay Later
- BNPL
- Financing
- Payments
- Credit
- Retail Finance
---
