---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thrivent.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.thrivent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thrivent Financial For Lutherans Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thrivent Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thrivent Financial
provider_slug: thrivent-financial-for-lutherans
slug: thrivent-financial-for-lutherans-domain-security
source_filename: thrivent-financial-for-lutherans-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thrivent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thrivent.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivent-financial-for-lutherans/refs/heads/main/security/thrivent-financial-for-lutherans-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Annuities
- Banking
- ETFs
- Financial Advice
- Financial Planning
- Fortune 500
- Generosity
- Insurance
- Investments
- Mutual Funds
- Non Profit
---
