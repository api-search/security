---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: island.is
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: devland.is
  spf: false
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: island.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 19:02:57 2026 GMT
  host: docs.devland.is
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.island.is
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Island Is Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for island.is (Digital Iceland), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: island.is (Digital Iceland)
provider_slug: island-is
slug: island-is-domain-security
source_filename: island-is-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: island.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.devland.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:02:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.island.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: island.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: devland.is\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/island-is/refs/heads/main/security/island-is-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Government
- GraphQL
- OpenAPI
- X-Road
- API Platform
- Government Data
- National Government
- Iceland
- Europe
---
