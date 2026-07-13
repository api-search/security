---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dune.com
  spf: true
hosts:
- cert_expires: Aug 14 20:09:10 2026 GMT
  host: dune.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 13:42:10 2026 GMT
  host: docs.dune.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:02:36 2026 GMT
  host: api.dune.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dune Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dune Analytics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dune Analytics
provider_slug: dune-analytics
slug: dune-analytics-domain-security
source_filename: dune-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 20:09:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.dune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 13:42:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:02:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dune.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dune-analytics/refs/heads/main/security/dune-analytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Analytics
- SQL
- Dashboards
- Blockchain
- Onchain
- Multi-chain
---
