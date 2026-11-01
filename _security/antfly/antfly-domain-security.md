---
api_specs:
- filename: antfly-ai-api-openapi.yml
  format: yaml
  label: Antfly AI API
  slug: antfly-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-ai-api-openapi.yml
- filename: antfly-cluster-management-api-openapi.yml
  format: yaml
  label: Antfly Cluster Management API
  slug: antfly-cluster-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-cluster-management-api-openapi.yml
- filename: antfly-data-operations-api-openapi.yml
  format: yaml
  label: Antfly Data Operations API
  slug: antfly-data-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-data-operations-api-openapi.yml
- filename: antfly-documents-api-openapi.yml
  format: yaml
  label: Antfly Documents API
  slug: antfly-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-documents-api-openapi.yml
- filename: antfly-index-management-api-openapi.yml
  format: yaml
  label: Antfly Index Management API
  slug: antfly-index-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-index-management-api-openapi.yml
- filename: antfly-inference-api-openapi.yml
  format: yaml
  label: Antfly Inference API
  slug: antfly-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-inference-api-openapi.yml
- filename: antfly-installed-api-openapi.yml
  format: yaml
  label: Antfly Installed API
  slug: antfly-installed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-installed-api-openapi.yml
- filename: antfly-memory-api-openapi.yml
  format: yaml
  label: Antfly Memory API
  slug: antfly-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-memory-api-openapi.yml
- filename: antfly-ml-api-openapi.yml
  format: yaml
  label: Antfly Ml API
  slug: antfly-ml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-ml-api-openapi.yml
- filename: antfly-models-api-openapi.yml
  format: yaml
  label: Antfly Models API
  slug: antfly-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-models-api-openapi.yml
- filename: antfly-packages-api-openapi.yml
  format: yaml
  label: Antfly Packages API
  slug: antfly-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-packages-api-openapi.yml
- filename: antfly-permission-api-openapi.yml
  format: yaml
  label: Antfly Permission API
  slug: antfly-permission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-permission-api-openapi.yml
- filename: antfly-personal-connections-api-openapi.yml
  format: yaml
  label: Antfly Personal Connections API
  slug: antfly-personal-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-personal-connections-api-openapi.yml
- filename: antfly-query-operations-api-openapi.yml
  format: yaml
  label: Antfly Query Operations API
  slug: antfly-query-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-query-operations-api-openapi.yml
- filename: antfly-resolver-curation-api-openapi.yml
  format: yaml
  label: Antfly Resolver Curation API
  slug: antfly-resolver-curation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-resolver-curation-api-openapi.yml
- filename: antfly-role-api-openapi.yml
  format: yaml
  label: Antfly Role API
  slug: antfly-role-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-role-api-openapi.yml
- filename: antfly-rowfilter-api-openapi.yml
  format: yaml
  label: Antfly Row Filter API
  slug: antfly-rowfilter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-rowfilter-api-openapi.yml
- filename: antfly-table-management-api-openapi.yml
  format: yaml
  label: Antfly Table Management API
  slug: antfly-table-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-table-management-api-openapi.yml
- filename: antfly-user-api-openapi.yml
  format: yaml
  label: Antfly User API
  slug: antfly-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-user-api-openapi.yml
- filename: antfly-api-key-api-openapi.yml
  format: yaml
  label: Antfly API Key API
  slug: antfly-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-api-key-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antfly.io
  spf: true
hosts:
- cert_expires: Dec 15 00:49:14 2026 GMT
  host: www.antfly.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Antfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antfly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Antfly
provider_slug: antfly
slug: antfly-domain-security
source_filename: antfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.antfly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 00:49:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: antfly.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/antfly/security/antfly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Search
- Retrieval
- Vector
- Hybrid
---
