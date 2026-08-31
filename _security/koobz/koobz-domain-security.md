---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: koo.bz
  spf: true
hosts:
- cert_expires: Oct  7 21:12:52 2026 GMT
  host: koo.bz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koobz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koobz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Koobz
provider_slug: koobz
slug: koobz-domain-security
source_filename: koobz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koo.bz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:12:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: koo.bz\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koobz/refs/heads/main/security/koobz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Footwear
- 3D Printing
- Additive Manufacturing
- Manufacturing
- Supply Chain
- Sustainability
- On Demand Manufacturing
- Dropshipping
- Circular Economy
---
