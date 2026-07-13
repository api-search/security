---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lendingclub.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.lendingclub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: developer.lendingclub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.lendingclub.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lendingclub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LendingClub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LendingClub
provider_slug: lendingclub
slug: lendingclub-domain-security
source_filename: lendingclub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lendingclub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lendingclub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lendingclub.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lendingclub.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendingclub/refs/heads/main/security/lendingclub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Personal Loans
- Banking
---
