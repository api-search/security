---
api_specs:
- filename: smartmind-file-api-openapi.yml
  format: yaml
  label: SmartMind file API
  slug: smartmind-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-file-api-openapi.yml
- filename: smartmind-health-api-openapi.yml
  format: yaml
  label: SmartMind health API
  slug: smartmind-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-health-api-openapi.yml
- filename: smartmind-metric-api-openapi.yml
  format: yaml
  label: SmartMind metric API
  slug: smartmind-metric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-metric-api-openapi.yml
- filename: smartmind-query-api-openapi.yml
  format: yaml
  label: SmartMind query API
  slug: smartmind-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-query-api-openapi.yml
- filename: smartmind-schema-api-openapi.yml
  format: yaml
  label: SmartMind schema API
  slug: smartmind-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-schema-api-openapi.yml
- filename: smartmind-table-api-openapi.yml
  format: yaml
  label: SmartMind table API
  slug: smartmind-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-table-api-openapi.yml
- filename: smartmind-table-template-api-openapi.yml
  format: yaml
  label: SmartMind table_template API
  slug: smartmind-table-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-table-template-api-openapi.yml
- filename: smartmind-view-api-openapi.yml
  format: yaml
  label: SmartMind view API
  slug: smartmind-view-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/openapi/smartmind-view-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smartmind-ai.io
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue " amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Oct 12 04:53:03 2026 GMT
  host: smartmind-ai.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: thanosql-sdk-python.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartMind, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SmartMind
provider_slug: smartmind
slug: smartmind-domain-security
source_filename: smartmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartmind-ai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: thanosql-sdk-python.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smartmind-ai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \" amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartmind/refs/heads/main/security/smartmind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Database
- Analytics
- Data
- SQL
- Ontology
- RAG
- Enterprise AI
---
