---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dragonflydb.io
  spf: true
hosts:
- cert_expires: Sep  3 03:41:15 2026 GMT
  host: www.dragonflydb.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dragonfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dragonfly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dragonfly
provider_slug: dragonfly
slug: dragonfly-domain-security
source_filename: dragonfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dragonflydb.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 03:41:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dragonflydb.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dragonfly/refs/heads/main/security/dragonfly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cache
- Database
- In-Memory
- Key-Value Store
- Redis
- Memcached
- Open Source
---
