---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prodpad.com
  spf: true
hosts:
- cert_expires: Sep 24 01:02:11 2026 GMT
  host: www.prodpad.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 12:53:51 2026 GMT
  host: help.prodpad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.prodpad.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Prodpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProdPad, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ProdPad
provider_slug: prodpad
slug: prodpad-domain-security
source_filename: prodpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prodpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:02:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.prodpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 12:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prodpad.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: prodpad.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodpad/refs/heads/main/security/prodpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Management
- Roadmaps
- Ideas
- Feedback
- OKRs
- Backlog
- Personas
---
