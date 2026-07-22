---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: soldsie.com
  spf: false
hosts:
- cert_expires: Oct 14 14:07:06 2026 GMT
  host: www.soldsie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soldsie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soldsie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Soldsie
provider_slug: soldsie
slug: soldsie-domain-security
source_filename: soldsie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soldsie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:07:06 2026 GMT\n  hsts: null\ndomains:\n- domain: soldsie.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soldsie/refs/heads/main/security/soldsie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social Commerce
- eCommerce
- Comment Selling
- Retail
- Facebook
- Instagram
- Defunct
---
