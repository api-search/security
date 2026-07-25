---
api_specs:
- filename: scylladb-account-api-openapi.yml
  format: yaml
  label: ScyllaDB Account API
  slug: scylladb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-account-api-openapi.yml
- filename: scylladb-account-cluster-network-api-openapi.yml
  format: yaml
  label: ScyllaDB Account Cluster Network API
  slug: scylladb-account-cluster-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-account-cluster-network-api-openapi.yml
- filename: scylladb-account-network-cluster-connection-api-openapi.yml
  format: yaml
  label: ScyllaDB Account network cluster connection API
  slug: scylladb-account-network-cluster-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-account-network-cluster-connection-api-openapi.yml
- filename: scylladb-cluster-api-openapi.yml
  format: yaml
  label: ScyllaDB Cluster API
  slug: scylladb-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-cluster-api-openapi.yml
- filename: scylladb-cluster-request-api-openapi.yml
  format: yaml
  label: ScyllaDB Cluster Request API
  slug: scylladb-cluster-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-cluster-request-api-openapi.yml
- filename: scylladb-deployment-api-openapi.yml
  format: yaml
  label: ScyllaDB Deployment API
  slug: scylladb-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-deployment-api-openapi.yml
- filename: scylladb-pricing-api-openapi.yml
  format: yaml
  label: ScyllaDB Pricing API
  slug: scylladb-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-pricing-api-openapi.yml
- filename: scylladb-vectorsearch-api-openapi.yml
  format: yaml
  label: ScyllaDB VectorSearch API
  slug: scylladb-vectorsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/openapi/scylladb-vectorsearch-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "amazonaws.com"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scylladb.com
  spf: true
hosts:
- cert_expires: Sep  8 14:25:23 2026 GMT
  host: www.scylladb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:36:48 2026 GMT
  host: cloud.docs.scylladb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 08:44:17 2026 GMT
  host: api.cloud.scylladb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scylladb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScyllaDB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ScyllaDB
provider_slug: scylladb
slug: scylladb-domain-security
source_filename: scylladb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scylladb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 14:25:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.docs.scylladb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:36:48 2026 GMT\n  hsts: false\n- host: api.cloud.scylladb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:44:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scylladb.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scylladb/refs/heads/main/security/scylladb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- NoSQL
- Cassandra Compatible
- DynamoDB Compatible
- Distributed Database
- Real-Time
- Vector Search
- Cloud Database
---
