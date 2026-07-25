---
api_specs:
- filename: artie-column-hashing-salts-api-openapi.yml
  format: yaml
  label: Artie Column Hashing Salts API
  slug: artie-column-hashing-salts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-column-hashing-salts-api-openapi.yml
- filename: artie-connectors-api-openapi.yml
  format: yaml
  label: Artie Connectors API
  slug: artie-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-connectors-api-openapi.yml
- filename: artie-data-catalog-api-openapi.yml
  format: yaml
  label: Artie Data Catalog API
  slug: artie-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-data-catalog-api-openapi.yml
- filename: artie-encryption-keys-api-openapi.yml
  format: yaml
  label: Artie Encryption Keys API
  slug: artie-encryption-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-encryption-keys-api-openapi.yml
- filename: artie-ingestion-api-keys-api-openapi.yml
  format: yaml
  label: Artie Ingestion API Keys API
  slug: artie-ingestion-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-ingestion-api-keys-api-openapi.yml
- filename: artie-pipelines-api-openapi.yml
  format: yaml
  label: Artie Pipelines API
  slug: artie-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-pipelines-api-openapi.yml
- filename: artie-privatelink-connections-api-openapi.yml
  format: yaml
  label: Artie PrivateLink Connections API
  slug: artie-privatelink-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-privatelink-connections-api-openapi.yml
- filename: artie-source-readers-api-openapi.yml
  format: yaml
  label: Artie Source Readers API
  slug: artie-source-readers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-source-readers-api-openapi.yml
- filename: artie-ssh-tunnels-api-openapi.yml
  format: yaml
  label: Artie SSH Tunnels API
  slug: artie-ssh-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/openapi/artie-ssh-tunnels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: artie.com
  spf: true
hosts:
- cert_expires: Sep  8 07:06:51 2026 GMT
  host: www.artie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 03:38:33 2026 GMT
  host: api.artie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artie, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Artie
provider_slug: artie
slug: artie-domain-security
source_filename: artie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 07:06:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.artie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:38:33 2026 GMT\n  hsts: null\ndomains:\n- domain: artie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artie/refs/heads/main/security/artie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Replication
- Change Data Capture
- Data Integration
- ETL
- Streaming
- Databases
- Data Warehouse
- CDC
- Data Engineering
---
