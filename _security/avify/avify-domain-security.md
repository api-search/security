---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avify.com
  spf: true
hosts:
- cert_expires: Oct 16 01:33:15 2026 GMT
  host: avify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 07:53:42 2026 GMT
  host: api.avify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avify
provider_slug: avify
slug: avify-domain-security
source_filename: avify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:33:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.avify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:53:42 2026 GMT\n  hsts: null\ndomains:\n- domain: avify.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avify/refs/heads/main/security/avify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- eCommerce
- CRM
- WhatsApp
- Conversational Commerce
- Inventory
- Point of Sale
- Payments
- Orders
- GraphQL
- Latin America
- SMB
---
