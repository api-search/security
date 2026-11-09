---
api_specs:
- filename: datasink-ing-documents-api-openapi.yml
  format: yaml
  label: DataSinking Documents API
  slug: datasink-ing-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-documents-api-openapi.yml
- filename: datasink-ing-exchanges-api-openapi.yml
  format: yaml
  label: DataSinking Exchanges API
  slug: datasink-ing-exchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-exchanges-api-openapi.yml
- filename: datasink-ing-feedback-api-openapi.yml
  format: yaml
  label: DataSinking Feedback API
  slug: datasink-ing-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-feedback-api-openapi.yml
- filename: datasink-ing-free-key-api-openapi.yml
  format: yaml
  label: DataSinking Free Key API
  slug: datasink-ing-free-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-free-key-api-openapi.yml
- filename: datasink-ing-stocks-api-openapi.yml
  format: yaml
  label: DataSinking Stocks API
  slug: datasink-ing-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-stocks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datasink.ing
  spf: true
hosts:
- cert_expires: Jan 21 07:46:30 2027 GMT
  host: datasink.ing
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datasink Ing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataSinking, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DataSinking
provider_slug: datasink-ing
slug: datasink-ing-domain-security
source_filename: datasink-ing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datasink.ing\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 07:46:30 2027 GMT\n  hsts: false\ndomains:\n- domain: datasink.ing\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datasink-ing/security/datasink-ing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Reports
- Markdown
- Data
---
