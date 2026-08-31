---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kinetica.com
  spf: true
hosts:
- cert_expires: Sep 28 07:20:15 2026 GMT
  host: www.kinetica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 14:32:38 2026 GMT
  host: docs.kinetica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 02:58:58 2026 GMT
  host: cloud.kinetica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kinetica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinetica, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kinetica
provider_slug: kinetica
slug: kinetica-domain-security
source_filename: kinetica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kinetica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:20:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.kinetica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.kinetica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 02:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kinetica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinetica/refs/heads/main/security/kinetica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Analytics
- gpu-acceleration
- real-time-analytics
- vector-search
- graph-analytics
- geospatial
- time-series
- SQL
- streaming
- data-infrastructure
- MCP
- agent-native
- RAG
---
