---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swn.com
  spf: true
- caa:
  - 0 iodef "mailto:itsecmon@expandenergy.com"
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expandenergy.com
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: www.swn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: ir.swn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:59:59 2026 GMT
  host: investors.expandenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Southwestern Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southwestern Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Southwestern Energy
provider_slug: southwestern-energy
slug: southwestern-energy-domain-security
source_filename: southwestern-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ir.swn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: null\n- host: investors.expandenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: swn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: expandenergy.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:itsecmon@expandenergy.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southwestern-energy/refs/heads/main/security/southwestern-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Natural Gas
- Energy
- Oil And Gas
---
