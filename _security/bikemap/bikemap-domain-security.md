---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bikemap.net
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: bikemap.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bikemap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bikemap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bikemap
provider_slug: bikemap
slug: bikemap-domain-security
source_filename: bikemap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bikemap.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bikemap.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bikemap/refs/heads/main/security/bikemap-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Cycling
- Navigation
- Maps
- Route Planning
- Mobility
- Outdoor
- Consumer App
---
