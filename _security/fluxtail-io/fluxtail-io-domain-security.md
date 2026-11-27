---
api_specs:
- filename: fluxtail-io-facets-api-openapi.yml
  format: yaml
  label: Fluxtail Facets API
  slug: fluxtail-io-facets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-facets-api-openapi.yml
- filename: fluxtail-io-histogram-api-openapi.yml
  format: yaml
  label: Fluxtail Histogram API
  slug: fluxtail-io-histogram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-histogram-api-openapi.yml
- filename: fluxtail-io-logs-api-openapi.yml
  format: yaml
  label: Fluxtail Logs API
  slug: fluxtail-io-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-logs-api-openapi.yml
- filename: fluxtail-io-receivers-api-openapi.yml
  format: yaml
  label: Fluxtail Receivers API
  slug: fluxtail-io-receivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxtail-io/openapi/fluxtail-io-receivers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fluxtail.io
  spf: true
hosts:
- cert_expires: Dec 17 07:50:41 2026 GMT
  host: fluxtail.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fluxtail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluxtail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fluxtail
provider_slug: fluxtail-io
slug: fluxtail-io-domain-security
source_filename: fluxtail-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluxtail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 07:50:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: fluxtail.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fluxtail-io/security/fluxtail-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logging
- Centralized
- MCP
- Artificial Intelligence
---
