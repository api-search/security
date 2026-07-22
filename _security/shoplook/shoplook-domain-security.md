---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shoplook.io
  spf: true
hosts:
- cert_expires: Sep 12 05:55:06 2026 GMT
  host: shoplook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shoplook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShopLook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShopLook
provider_slug: shoplook
slug: shoplook-domain-security
source_filename: shoplook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shoplook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:55:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shoplook.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shoplook/refs/heads/main/security/shoplook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fashion
- E-commerce
- Styling
- Shopping
- Outfits
- Social
- Mobile App
- AI Stylist
---
