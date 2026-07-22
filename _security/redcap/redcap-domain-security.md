---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getredcap.com
  spf: true
- caa:
  - 0 issue "pki.goog cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "pki.goog"
  - 0 issuewild "ssl.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: solera.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.getredcap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 22:04:11 2026 GMT
  host: www.servicesuite.solera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redcap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RedCap, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: RedCap
provider_slug: redcap
slug: redcap-domain-security
source_filename: redcap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getredcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.servicesuite.solera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:04:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getredcap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: solera.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redcap/refs/heads/main/security/redcap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Automotive
- Dealership
- Service
- Fixed Operations
- Pickup and Delivery
- Logistics
---
