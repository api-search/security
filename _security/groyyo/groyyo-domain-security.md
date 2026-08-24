---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groyyo.com
  spf: true
hosts:
- cert_expires: Sep 21 03:53:37 2026 GMT
  host: groyyo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groyyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groyyo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Groyyo
provider_slug: groyyo
slug: groyyo-domain-security
source_filename: groyyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groyyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:53:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: groyyo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groyyo/refs/heads/main/security/groyyo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Supply Chain
- Apparel
- Fashion
- Sourcing
- B2B
- ERP
- Quality Control
- India
---
