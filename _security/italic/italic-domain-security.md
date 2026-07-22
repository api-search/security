---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: italic.com
  spf: true
hosts:
- cert_expires: Sep 16 13:49:32 2026 GMT
  host: italic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Italic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Italic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Italic
provider_slug: italic
slug: italic-domain-security
source_filename: italic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: italic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:49:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: italic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/italic/refs/heads/main/security/italic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Retail
- Consumer
- Home Goods
- Direct-to-Consumer
- Marketplace
- Membership
---
