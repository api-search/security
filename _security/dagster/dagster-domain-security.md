---
api_specs:
- filename: dagster-external-assets-rest-api-openapi.yml
  format: yaml
  label: Dagster External Assets REST API
  slug: external-assets-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/openapi/dagster-external-assets-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dagster.cloud
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dagster.io
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: dagster.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 06:56:25 2026 GMT
  host: docs.dagster.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dagster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dagster, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dagster
provider_slug: dagster
slug: dagster-domain-security
source_filename: dagster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dagster.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dagster.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 06:56:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dagster.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: dagster.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/security/dagster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Engineering
- Data Orchestration
- Data Pipelines
- ETL
- Workflows
- Assets
- GraphQL
---
