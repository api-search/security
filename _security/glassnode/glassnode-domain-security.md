---
api_specs:
- filename: glassnode-openapi.yml
  format: yaml
  label: Glassnode Metrics API
  slug: metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/openapi/glassnode-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: glassnode.com
  spf: true
hosts:
- cert_expires: Sep 19 19:51:11 2026 GMT
  host: glassnode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 05:49:07 2026 GMT
  host: docs.glassnode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 16:35:52 2026 GMT
  host: api.glassnode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glassnode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glassnode, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Glassnode
provider_slug: glassnode
slug: glassnode-domain-security
source_filename: glassnode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glassnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:51:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.glassnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 05:49:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.glassnode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:35:52 2026 GMT\n  hsts: null\ndomains:\n- domain: glassnode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glassnode/refs/heads/main/security/glassnode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Crypto
- On-Chain
- Analytics
- Metrics
- Bitcoin
- Ethereum
- Institutional
---
