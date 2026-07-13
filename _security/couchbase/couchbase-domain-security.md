---
api_specs:
- filename: couchbase-server-rest-api-openapi.yml
  format: yaml
  label: Couchbase Server REST API
  slug: couchbase-server-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-server-rest-api-openapi.yml
- filename: couchbase-query-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Query Service REST API
  slug: couchbase-query-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-query-service-rest-api-openapi.yml
- filename: couchbase-analytics-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Analytics Service REST API
  slug: couchbase-analytics-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-analytics-service-rest-api-openapi.yml
- filename: couchbase-search-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Search Service REST API
  slug: couchbase-search-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-search-service-rest-api-openapi.yml
- filename: couchbase-eventing-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Eventing Service REST API
  slug: couchbase-eventing-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-eventing-service-rest-api-openapi.yml
- filename: couchbase-backup-service-rest-api-openapi.yml
  format: yaml
  label: Couchbase Backup Service REST API
  slug: couchbase-backup-service-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-backup-service-rest-api-openapi.yml
- filename: couchbase-xdcr-rest-api-openapi.yml
  format: yaml
  label: Couchbase XDCR REST API
  slug: couchbase-xdcr-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-xdcr-rest-api-openapi.yml
- filename: couchbase-capella-management-api-openapi.yml
  format: yaml
  label: Couchbase Capella Management API
  slug: couchbase-capella-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-capella-management-api-openapi.yml
- filename: couchbase-capella-app-services-public-api-openapi.yml
  format: yaml
  label: Couchbase Capella App Services Public API
  slug: couchbase-capella-app-services-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-capella-app-services-public-api-openapi.yml
- filename: couchbase-capella-app-services-admin-api-openapi.yml
  format: yaml
  label: Couchbase Capella App Services Admin API
  slug: couchbase-capella-app-services-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-capella-app-services-admin-api-openapi.yml
- filename: couchbase-sync-gateway-public-rest-api-openapi.yml
  format: yaml
  label: Couchbase Sync Gateway Public REST API
  slug: couchbase-sync-gateway-public-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-sync-gateway-public-rest-api-openapi.yml
- filename: couchbase-sync-gateway-admin-rest-api-openapi.yml
  format: yaml
  label: Couchbase Sync Gateway Admin REST API
  slug: couchbase-sync-gateway-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/openapi/couchbase-sync-gateway-admin-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: couchbase.com
  spf: true
hosts:
- cert_expires: Jul 22 20:03:55 2026 GMT
  host: www.couchbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: docs.couchbase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 00:14:43 2026 GMT
  host: cloudapi.cloud.couchbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Couchbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Couchbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Couchbase
provider_slug: couchbase
slug: couchbase-domain-security
source_filename: couchbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.couchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 22 20:03:55 2026 GMT\n  hsts: false\n- host: docs.couchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: cloudapi.cloud.couchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:14:43 2026 GMT\n  hsts: null\ndomains:\n- domain: couchbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/couchbase/refs/heads/main/security/couchbase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- App Services
- Backup
- Capella
- Cloud
- Database
- DBaaS
- Eventing
- Full-Text Search
- Gateway
- JSON
- Mobile
- NoSQL
- Replication
- SQL++
- Sync
- Vector Search
- XDCR
---
