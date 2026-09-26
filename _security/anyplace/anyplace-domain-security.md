---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anyplace.com
  spf: true
hosts:
- cert_expires: Nov 25 10:59:51 2026 GMT
  host: www.anyplace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 11:45:28 2026 GMT
  host: dev.anyplace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Anyplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anyplace, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anyplace
provider_slug: anyplace
slug: anyplace-domain-security
source_filename: anyplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anyplace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 10:59:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.anyplace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 11:45:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anyplace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyplace/refs/heads/main/security/anyplace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Housing
- RemoteWork
- FlexibleLease
- Apartments
---
