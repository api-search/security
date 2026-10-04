---
api_specs:
- filename: informatica-authentication-api-openapi.yml
  format: yaml
  label: Informatica Authentication API
  slug: informatica-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-authentication-api-openapi.yml
- filename: informatica-connections-api-openapi.yml
  format: yaml
  label: Informatica Connections API
  slug: informatica-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-connections-api-openapi.yml
- filename: informatica-jobs-api-openapi.yml
  format: yaml
  label: Informatica Jobs API
  slug: informatica-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-jobs-api-openapi.yml
- filename: informatica-mapping-tasks-api-openapi.yml
  format: yaml
  label: Informatica Mapping Tasks API
  slug: informatica-mapping-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-mapping-tasks-api-openapi.yml
- filename: informatica-mappings-api-openapi.yml
  format: yaml
  label: Informatica Mappings API
  slug: informatica-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-mappings-api-openapi.yml
- filename: informatica-schedules-api-openapi.yml
  format: yaml
  label: Informatica Schedules API
  slug: informatica-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-schedules-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: informatica.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.informatica.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 15:53:28 2026 GMT
  host: developer.informatica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: docs.informatica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Informatica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Informatica, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Informatica
provider_slug: informatica
slug: informatica-domain-security
source_filename: informatica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.informatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2628000\n- host: developer.informatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 15:53:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.informatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: informatica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/security/informatica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
- Data Catalog
---
