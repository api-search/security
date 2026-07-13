---
api_specs:
- filename: dbnomics-openapi.yml
  format: yaml
  label: DBnomics Providers API
  slug: dbnomics-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbnomics/refs/heads/main/openapi/dbnomics-openapi.yml
- filename: dbnomics-openapi.yml
  format: yaml
  label: DBnomics Datasets API
  slug: dbnomics-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbnomics/refs/heads/main/openapi/dbnomics-openapi.yml
- filename: dbnomics-openapi.yml
  format: yaml
  label: DBnomics Series API
  slug: dbnomics-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbnomics/refs/heads/main/openapi/dbnomics-openapi.yml
- filename: dbnomics-openapi.yml
  format: yaml
  label: DBnomics Search API
  slug: dbnomics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dbnomics/refs/heads/main/openapi/dbnomics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomics.world
  spf: true
hosts:
- cert_expires: Aug 30 14:31:31 2026 GMT
  host: db.nomics.world
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 04:00:17 2026 GMT
  host: api.db.nomics.world
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dbnomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DBnomics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DBnomics
provider_slug: dbnomics
slug: dbnomics-domain-security
source_filename: dbnomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: db.nomics.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:31:31 2026 GMT\n  hsts: false\n- host: api.db.nomics.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:00:17 2026 GMT\n  hsts: null\ndomains:\n- domain: nomics.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dbnomics/refs/heads/main/security/dbnomics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Economic Indicators
- Macroeconomics
- Open Data
- Statistics
- Time Series
- Government Data
---
