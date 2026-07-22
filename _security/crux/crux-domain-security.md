---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: crux.com
  spf: false
hosts:
- cert_expires: Sep 24 20:35:42 2026 GMT
  host: www.crux.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Crux
provider_slug: crux
slug: crux-domain-security
source_filename: crux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crux.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:35:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crux.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crux/refs/heads/main/security/crux-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Clean Energy
- Climate Finance
- Tax Credits
- Capital Markets
- Fintech
- Energy
- Marketplace
- Sustainability
---
