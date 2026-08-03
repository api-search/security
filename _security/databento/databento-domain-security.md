---
api_specs:
- filename: databento-timeseries-api-openapi.yml
  format: yaml
  label: Databento Historical Timeseries API
  slug: databento-historical-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-timeseries-api-openapi.yml
- filename: databento-metadata-api-openapi.yml
  format: yaml
  label: Databento Metadata API
  slug: databento-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-metadata-api-openapi.yml
- filename: databento-symbology-api-openapi.yml
  format: yaml
  label: Databento Symbology API
  slug: databento-symbology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-symbology-api-openapi.yml
- filename: databento-batch-api-openapi.yml
  format: yaml
  label: Databento Batch API
  slug: databento-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-batch-api-openapi.yml
- filename: databento-reference-api-openapi.yml
  format: yaml
  label: Databento Reference API
  slug: databento-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-reference-api-openapi.yml
- filename: databento-platform-openapi-official.json
  format: json
  label: Databento OpenAPI specification
  slug: databento-platform-openapi-official
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/openapi/databento-platform-openapi-official.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: databento.com
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: databento.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 12:56:09 2026 GMT
  host: hist.databento.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: glbx.mdp3.lsg.databento.com
  https: false
kind: domain-security
layout: security
method: probed
name: Databento Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databento, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Databento
provider_slug: databento
slug: databento-domain-security
source_filename: databento-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: databento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: hist.databento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:56:09 2026 GMT\n  hsts: null\n- host: glbx.mdp3.lsg.databento.com\n  https: false\ndomains:\n- domain: databento.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databento/refs/heads/main/security/databento-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Market Data
- Financial Data
- Reference Data
- Historical Market Data
- Trading
---
