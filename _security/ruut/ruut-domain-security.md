---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ruut.mx
  spf: true
hosts:
- cert_expires: Oct  6 21:37:05 2026 GMT
  host: ruut.mx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ruut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RUUT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RUUT
provider_slug: ruut
slug: ruut-domain-security
source_filename: ruut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ruut.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:37:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ruut.mx\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ruut/refs/heads/main/security/ruut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Fintech
- Investing
- Investment Platform
- Wealth Management
- Stocks
- Mexico
---
