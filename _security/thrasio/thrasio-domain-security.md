---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thrasio.com
  spf: true
hosts:
- cert_expires: Sep 29 13:40:34 2026 GMT
  host: www.thrasio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thrasio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thrasio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thrasio
provider_slug: thrasio
slug: thrasio-domain-security
source_filename: thrasio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thrasio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:40:34 2026 GMT\n  hsts: false\ndomains:\n- domain: thrasio.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrasio/refs/heads/main/security/thrasio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Consumer Goods
- Retail
- Marketplace
- Brands
- Amazon
---
