---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: univer.se
  spf: true
hosts:
- cert_expires: Aug 25 04:09:21 2026 GMT
  host: univer.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Universe
provider_slug: universe
slug: universe-domain-security
source_filename: universe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: univer.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:09:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: univer.se\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universe/refs/heads/main/security/universe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Website Builder
- No-Code
- eCommerce
- Creator Economy
- Small Business
- Mobile
---
