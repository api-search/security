---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hoppscotch.com
  spf: false
hosts:
- cert_expires: Aug 24 21:50:51 2026 GMT
  host: hoppscotch.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hoppscotch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hoppscotch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Hoppscotch
provider_slug: hoppscotch
slug: hoppscotch-domain-security
source_filename: hoppscotch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoppscotch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 21:50:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: hoppscotch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hoppscotch/refs/heads/main/security/hoppscotch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Testing
- Clients
- GraphQL
- Open Source
- Platform
- REST
- WebSockets
---
