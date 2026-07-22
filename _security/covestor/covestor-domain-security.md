---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "geotrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: covestor.com
  spf: true
hosts:
- cert_expires: Sep 20 09:59:41 2026 GMT
  host: covestor.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covestor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covestor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Covestor
provider_slug: covestor
slug: covestor-domain-security
source_filename: covestor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covestor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:59:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: covestor.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"geotrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covestor/refs/heads/main/security/covestor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Investing
- Wealth Management
- Brokerage
- Social Investing
- Acquired
---
