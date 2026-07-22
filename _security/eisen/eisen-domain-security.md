---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 iodef "mailto:security@witheisen.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: witheisen.com
  spf: true
hosts:
- cert_expires: Oct  7 12:35:08 2026 GMT
  host: www.witheisen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eisen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eisen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eisen
provider_slug: eisen
slug: eisen-domain-security
source_filename: eisen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.witheisen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: witheisen.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 iodef \"mailto:security@witheisen.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eisen/refs/heads/main/security/eisen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Compliance
- Escheatment
- Unclaimed Property
- Financial Services
- RegTech
- Disbursements
- Tax Reporting
- Fintech
---
