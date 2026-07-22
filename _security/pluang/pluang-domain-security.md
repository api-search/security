---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazon.com"
  - 0 issue ";"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pluang.com
  spf: true
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: pluang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pluang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pluang, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pluang
provider_slug: pluang
slug: pluang-domain-security
source_filename: pluang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pluang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pluang.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \";\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluang/refs/heads/main/security/pluang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fintech
- Investing
- Trading
- Cryptocurrency
- Stocks
- Wealth Management
- Indonesia
---
