---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: packagingcorp.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: www.packagingcorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Packaging Corp Of America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Packaging Corporation of America, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Packaging Corporation of America
provider_slug: packaging-corp-of-america
slug: packaging-corp-of-america-domain-security
source_filename: packaging-corp-of-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.packagingcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: packagingcorp.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/packaging-corp-of-america/refs/heads/main/security/packaging-corp-of-america-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Containerboard
- Corrugated Packaging
- Fortune 500
- Manufacturing
- Packaging
---
