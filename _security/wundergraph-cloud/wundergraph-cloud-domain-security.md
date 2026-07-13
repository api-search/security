---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wundergraph.com
  spf: true
hosts:
- cert_expires: Aug 24 10:40:42 2026 GMT
  host: wundergraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:38:55 2026 GMT
  host: cosmo-docs.wundergraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:35:52 2026 GMT
  host: cosmo-cp.wundergraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wundergraph Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WunderGraph Cloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WunderGraph Cloud
provider_slug: wundergraph-cloud
slug: wundergraph-cloud-domain-security
source_filename: wundergraph-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wundergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:40:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cosmo-docs.wundergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:38:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cosmo-cp.wundergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:35:52 2026 GMT\n  hsts: null\ndomains:\n- domain: wundergraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wundergraph-cloud/refs/heads/main/security/wundergraph-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Federation
- API Gateway
- Supergraph
- API Management
- GraphQL Federation
- Developer Platform
---
