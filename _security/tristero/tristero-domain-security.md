---
api_specs:
- filename: tristero-api-openapi.json
  format: json
  label: Tristero API
  slug: tristero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-api-openapi.json
- filename: tristero-feather-api-openapi.json
  format: json
  label: Feather API
  slug: feather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/openapi/tristero-feather-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tristero.com
  spf: true
hosts:
- cert_expires: Oct 18 01:00:03 2026 GMT
  host: tristero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 01:00:03 2026 GMT
  host: docs.tristero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 02:03:09 2026 GMT
  host: api.tristero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tristero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tristero, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tristero
provider_slug: tristero
slug: tristero-domain-security
source_filename: tristero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tristero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:00:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tristero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:00:03 2026 GMT\n  hsts: false\n- host: api.tristero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:03:09 2026 GMT\n  hsts: null\ndomains:\n- domain: tristero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tristero/refs/heads/main/security/tristero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Trading
- DeFi
- Cross-Chain
- Web3
- Margin Trading
- Dark Pools
---
