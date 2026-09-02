---
api_specs:
- filename: lakekeeper-generic-table-api-openapi.yml
  format: yaml
  label: Lakekeeper Generic Table (Data) API
  slug: lakekeeper-generic-table-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-generic-table-api-openapi.yml
- filename: lakekeeper-authorization-api-openapi.yml
  format: yaml
  label: Lakekeeper Authorization API
  slug: lakekeeper-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-authorization-api-openapi.yml
- filename: lakekeeper-catalog-api-api-openapi.yml
  format: yaml
  label: Lakekeeper Catalog API
  slug: lakekeeper-catalog-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-catalog-api-api-openapi.yml
- filename: lakekeeper-configuration-api-api-openapi.yml
  format: yaml
  label: Lakekeeper Configuration API
  slug: lakekeeper-configuration-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-configuration-api-api-openapi.yml
- filename: lakekeeper-oauth2-api-api-openapi.yml
  format: yaml
  label: Lakekeeper OAuth2 API
  slug: lakekeeper-oauth2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-oauth2-api-api-openapi.yml
- filename: lakekeeper-permissions-cedar-api-openapi.yml
  format: yaml
  label: Lakekeeper Permissions Cedar API
  slug: lakekeeper-permissions-cedar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-permissions-cedar-api-openapi.yml
- filename: lakekeeper-permissions-openfga-api-openapi.yml
  format: yaml
  label: Lakekeeper Permissions Openfga API
  slug: lakekeeper-permissions-openfga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-permissions-openfga-api-openapi.yml
- filename: lakekeeper-project-api-openapi.yml
  format: yaml
  label: Lakekeeper Project API
  slug: lakekeeper-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-project-api-openapi.yml
- filename: lakekeeper-role-api-openapi.yml
  format: yaml
  label: Lakekeeper Role API
  slug: lakekeeper-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-role-api-openapi.yml
- filename: lakekeeper-server-api-openapi.yml
  format: yaml
  label: Lakekeeper Server API
  slug: lakekeeper-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-server-api-openapi.yml
- filename: lakekeeper-tasks-api-openapi.yml
  format: yaml
  label: Lakekeeper Tasks API
  slug: lakekeeper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-tasks-api-openapi.yml
- filename: lakekeeper-user-api-openapi.yml
  format: yaml
  label: Lakekeeper User API
  slug: lakekeeper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-user-api-openapi.yml
- filename: lakekeeper-warehouse-api-openapi.yml
  format: yaml
  label: Lakekeeper Warehouse API
  slug: lakekeeper-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-warehouse-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lakekeeper.io
  spf: false
hosts:
- cert_expires: Oct 22 10:39:59 2026 GMT
  host: lakekeeper.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 01:09:19 2026 GMT
  host: docs.lakekeeper.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lakekeeper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lakekeeper, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lakekeeper
provider_slug: lakekeeper
slug: lakekeeper-domain-security
source_filename: lakekeeper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lakekeeper.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 10:39:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.lakekeeper.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 01:09:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: lakekeeper.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/security/lakekeeper-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Apache Iceberg
- Data Catalog
- Lakehouse
- Open-Source
- Rust
- Data Governance
- Access Control
- Object Storage
- Metadata
- Self-Hosted
- openfga
- Data Engineering
---
