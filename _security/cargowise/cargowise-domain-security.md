---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cargowise.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "certainly.com"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wisetechacademy.com
  spf: true
hosts:
- cert_expires: Oct  5 06:54:29 2026 GMT
  host: www.cargowise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 01:13:45 2026 GMT
  host: wisetechacademy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:48:10 2026 GMT
  host: www.scribd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cargowise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CargoWise, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CargoWise
provider_slug: cargowise
slug: cargowise-domain-security
source_filename: cargowise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cargowise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 06:54:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wisetechacademy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 01:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.scribd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cargowise.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wisetechacademy.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargowise/refs/heads/main/security/cargowise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Freight Forwarding
- Supply Chain
- Customs
- Shipping
- eAdaptor
- Universal XML
- EDI
- WiseTech Global
---
