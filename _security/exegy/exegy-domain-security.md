---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issuewild "usertrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: exegy.com
  spf: true
hosts:
- cert_expires: Aug 11 01:24:12 2026 GMT
  host: www.exegy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 15:33:14 2026 GMT
  host: exegy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exegy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exegy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Exegy
provider_slug: exegy
slug: exegy-domain-security
source_filename: exegy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exegy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 01:24:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: exegy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:33:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exegy.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exegy/refs/heads/main/security/exegy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Trading
- Real-Time
- Low Latency
- FPGA
- Options
- Feed Handlers
- Order Book
---
