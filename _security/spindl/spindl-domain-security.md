---
api_specs:
- filename: spindl-events-api-openapi.yml
  format: yaml
  label: Spindl Events API
  slug: spindl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-events-api-openapi.yml
- filename: spindl-short-links-api-openapi.yml
  format: yaml
  label: Spindl Short Links API
  slug: spindl-short-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-short-links-api-openapi.yml
- filename: spindl-ads-api-openapi.yml
  format: yaml
  label: Spindl Ads API
  slug: spindl-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-ads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spindl.xyz
  spf: true
hosts:
- cert_expires: Sep 16 13:55:36 2026 GMT
  host: spindl.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 14:44:41 2026 GMT
  host: docs.spindl.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: api.spindl.xyz
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spindl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spindl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spindl
provider_slug: spindl
slug: spindl-domain-security
source_filename: spindl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spindl.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:55:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.spindl.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 14:44:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.spindl.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spindl.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/security/spindl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Attribution
- Analytics
- Marketing
- Growth
- SDK
- Web3
---
