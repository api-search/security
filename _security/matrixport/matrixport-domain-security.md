---
api_specs:
- filename: matrixport-bitcom-openapi.yml
  format: yaml
  label: bit.com v1 API
  slug: bitcom-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/openapi/matrixport-bitcom-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bit.com
  spf: true
hosts:
- cert_expires: Sep 20 05:25:06 2026 GMT
  host: www.bit.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: api.bit.com
  https: false
kind: domain-security
layout: security
method: probed
name: Matrixport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matrixport, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Matrixport
provider_slug: matrixport
slug: matrixport-domain-security
source_filename: matrixport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.bit.com\n  https: false\ndomains:\n- domain: bit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrixport/refs/heads/main/security/matrixport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Finance
- Cryptocurrency Exchange
- Trading
- Derivatives
- Options
- Futures
- Perpetuals
- WebSocket
- REST API
---
