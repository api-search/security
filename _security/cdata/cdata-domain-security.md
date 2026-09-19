---
api_specs:
- filename: cdata-mcp-api-openapi.yml
  format: yaml
  label: CData Connect AI MCP Server
  slug: mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-mcp-api-openapi.yml
- filename: cdata-account-api-openapi.yml
  format: yaml
  label: CData Account API
  slug: cdata-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-account-api-openapi.yml
- filename: cdata-cache-api-openapi.yml
  format: yaml
  label: CData Cache API
  slug: cdata-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-cache-api-openapi.yml
- filename: cdata-connection-api-openapi.yml
  format: yaml
  label: CData Connection API
  slug: cdata-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-connection-api-openapi.yml
- filename: cdata-data-explorer-api-openapi.yml
  format: yaml
  label: CData Data Explorer API
  slug: cdata-data-explorer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-data-explorer-api-openapi.yml
- filename: cdata-job-api-openapi.yml
  format: yaml
  label: CData Job API
  slug: cdata-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-job-api-openapi.yml
- filename: cdata-jobs-api-openapi.yml
  format: yaml
  label: CData Jobs API
  slug: cdata-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-jobs-api-openapi.yml
- filename: cdata-log-api-openapi.yml
  format: yaml
  label: CData Log API
  slug: cdata-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-log-api-openapi.yml
- filename: cdata-metadata-api-openapi.yml
  format: yaml
  label: CData Metadata API
  slug: cdata-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-metadata-api-openapi.yml
- filename: cdata-query-api-openapi.yml
  format: yaml
  label: CData Query API
  slug: cdata-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-query-api-openapi.yml
- filename: cdata-service-accounts-api-openapi.yml
  format: yaml
  label: CData Service Accounts API
  slug: cdata-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-service-accounts-api-openapi.yml
- filename: cdata-users-api-openapi.yml
  format: yaml
  label: CData Users API
  slug: cdata-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-users-api-openapi.yml
- filename: cdata-odata-api-openapi.yml
  format: yaml
  label: CData O Data API
  slug: cdata-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-odata-api-openapi.yml
- filename: cdata-open-api-api-openapi.yml
  format: yaml
  label: CData Open API
  slug: cdata-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/openapi/cdata-open-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cdata.com
  spf: true
hosts:
- cert_expires: Nov  1 08:33:29 2026 GMT
  host: www.cdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 01:18:23 2026 GMT
  host: cloud.cdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 01:18:23 2026 GMT
  host: mcp.cloud.cdata.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'The automated probe recorded hsts: null because the host answers 404 at "/". A direct check on 2026-09-05 confirms the header is present on both GET / (404) and the MCP endpoint''s 401 challenge: strict-transport-security: max-age=31536000; includeSubDomains. Corrected by hand rather than left as a false negative.'
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CData, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CData
provider_slug: cdata
slug: cdata-domain-security
source_filename: cdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 08:33:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.cdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 01:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.cloud.cdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 01:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    The automated probe recorded hsts: null because the host answers 404 at \"/\". A direct\n    check on 2026-09-05 confirms the header is present on both GET / (404) and the MCP\n    endpoint's 401 challenge: strict-transport-security: max-age=31536000; includeSubDomains.\n    Corrected by hand rather than left as a false negative.\ndomains:\n- domain: cdata.com\n  dnssec: false\n \
  \ caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdata/refs/heads/main/security/cdata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Data Access
- Data Connectivity
- Database
- NoSQL
- SQL
---
