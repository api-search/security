---
api_specs:
- filename: abbyy-catalogrecords-api-openapi.yml
  format: yaml
  label: ABBYY Catalog Records API
  slug: abbyy-catalogrecords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-catalogrecords-api-openapi.yml
- filename: abbyy-catalogs-api-openapi.yml
  format: yaml
  label: ABBYY Catalogs API
  slug: abbyy-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-catalogs-api-openapi.yml
- filename: abbyy-invites-api-openapi.yml
  format: yaml
  label: ABBYY Invites API
  slug: abbyy-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-invites-api-openapi.yml
- filename: abbyy-report-api-openapi.yml
  format: yaml
  label: ABBYY Report API
  slug: abbyy-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-report-api-openapi.yml
- filename: abbyy-report-v1-api-openapi.yml
  format: yaml
  label: ABBYY Report v1 API
  slug: abbyy-report-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-report-v1-api-openapi.yml
- filename: abbyy-skills-api-openapi.yml
  format: yaml
  label: ABBYY Skills API
  slug: abbyy-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-skills-api-openapi.yml
- filename: abbyy-transactions-api-openapi.yml
  format: yaml
  label: ABBYY Transactions API
  slug: abbyy-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-transactions-api-openapi.yml
- filename: abbyy-transaction-documents-api-openapi.yml
  format: yaml
  label: ABBYY Transaction Documents API
  slug: abbyy-transaction-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/openapi/abbyy-transaction-documents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abbyy.com
  spf: true
hosts:
- cert_expires: Nov 17 07:50:50 2026 GMT
  host: www.abbyy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:34:09 2026 GMT
  host: docs.abbyy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 14:09:36 2026 GMT
  host: vantage-us.abbyy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Abbyy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABBYY, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ABBYY
provider_slug: abbyy
slug: abbyy-domain-security
source_filename: abbyy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abbyy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 07:50:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.abbyy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:34:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: vantage-us.abbyy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 14:09:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abbyy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbyy/refs/heads/main/security/abbyy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Automation
- Document Processing
- OCR
- Intelligent Document Processing
- Data Extraction
- Process Intelligence
- MCP
- Agent Skills
- RPA
- Enterprise Automation
- A2A
---
