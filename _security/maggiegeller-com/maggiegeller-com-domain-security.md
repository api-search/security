---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maggiegeller.com
  spf: true
hosts:
- cert_expires: Jan 11 00:18:39 2027 GMT
  host: maggiegeller.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dr. Maggie Geller, OD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dr. Maggie Geller, OD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dr. Maggie Geller, OD
provider_slug: maggiegeller-com
slug: maggiegeller-com-domain-security
source_filename: maggiegeller-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maggiegeller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 00:18:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maggiegeller.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/maggiegeller-com/security/maggiegeller-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Optometry
- Healthcare
- Vision Care
- MyopiaManagement
- DryEyeTherapy
---
