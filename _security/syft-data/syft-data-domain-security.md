---
api_specs:
- filename: syft-data-export-api-openapi.yml
  format: yaml
  label: Syft Data Export API
  slug: syft-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-export-api-openapi.yml
- filename: syft-data-lookup-api-openapi.yml
  format: yaml
  label: Syft Data Lookup API
  slug: syft-data-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-lookup-api-openapi.yml
- filename: syft-data-events-api-openapi.yml
  format: yaml
  label: Syft Data Event Collection API
  slug: syft-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/openapi/syft-data-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: syftdata.com
  spf: true
hosts:
- cert_expires: Sep 21 00:38:59 2026 GMT
  host: www.syftdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 22:06:54 2026 GMT
  host: docs.syftdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 06:08:10 2026 GMT
  host: app.syftdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syft Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syft Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Syft Data
provider_slug: syft-data
slug: syft-data-domain-security
source_filename: syft-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syftdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:38:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.syftdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:06:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.syftdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 06:08:10 2026 GMT\n  hsts: null\ndomains:\n- domain: syftdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syft-data/refs/heads/main/security/syft-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lead Intelligence
- Intent Data
- Website Visitor Identification
- Sales Intelligence
- Go-To-Market
- Analytics
- MCP
---
