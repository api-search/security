---
description: ''
domains:
- caa:
  - 128 issuewild "sectigo.com"
  - 128 issue "digicert.com"
  - 128 issue "sectigo.com"
  - 128 issuewild "digicert.com"
  - 0 issue "digicert.com"
  - 128 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: synchronoss.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: synchronoss.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synchronoss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synchronoss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Synchronoss
provider_slug: synchronoss
slug: synchronoss-domain-security
source_filename: synchronoss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synchronoss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synchronoss.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"sectigo.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 128 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synchronoss/refs/heads/main/security/synchronoss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Personal Cloud
- Messaging
- Telecommunications
- White Label
- Data Backup
- Carrier Services
---
