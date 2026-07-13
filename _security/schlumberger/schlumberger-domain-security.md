---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 iodef "mailto:pki-admin-manager@slb.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slb.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.slb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:43:08 2026 GMT
  host: developer.slb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: api.slb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schlumberger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SLB (Schlumberger), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SLB (Schlumberger)
provider_slug: schlumberger
slug: schlumberger-domain-security
source_filename: schlumberger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.slb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:43:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.slb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: slb.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 iodef \"mailto:pki-admin-manager@slb.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schlumberger/refs/heads/main/security/schlumberger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oilfield Services
---
