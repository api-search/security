---
api_specs:
- filename: infoworks-rest-api-v3-openapi.yml
  format: yaml
  label: Infoworks REST API v3
  slug: infoworks-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infoworks/refs/heads/main/openapi/infoworks-rest-api-v3-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uniphore.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infoworks.io
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.uniphore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 08:46:34 2026 GMT
  host: docs.infoworks.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Infoworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infoworks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Infoworks
provider_slug: infoworks
slug: infoworks-domain-security
source_filename: infoworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uniphore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: docs.infoworks.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 08:46:34 2026 GMT\n  hsts: false\ndomains:\n- domain: uniphore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: infoworks.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infoworks/refs/heads/main/security/infoworks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Data Engineering
- Data Integration
- Data Ingestion
- Data Pipelines
- Workflow Orchestration
- Data Warehouse Modernization
- Databricks
- Snowflake
- Big Data
- ETL
- Enterprise Data Operations
- Self-Hosted
---
