---
api_specs:
- filename: amazon-aurora-db-cluster-endpoints-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Cluster Endpoints API
  slug: amazon-aurora-db-cluster-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-cluster-endpoints-api-openapi.yml
- filename: amazon-aurora-db-cluster-parameter-groups-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Cluster Parameter Groups API
  slug: amazon-aurora-db-cluster-parameter-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-cluster-parameter-groups-api-openapi.yml
- filename: amazon-aurora-db-cluster-snapshots-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Cluster Snapshots API
  slug: amazon-aurora-db-cluster-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-cluster-snapshots-api-openapi.yml
- filename: amazon-aurora-db-clusters-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Clusters API
  slug: amazon-aurora-db-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-clusters-api-openapi.yml
- filename: amazon-aurora-db-instances-api-openapi.yml
  format: yaml
  label: Amazon Aurora DB Instances API
  slug: amazon-aurora-db-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-db-instances-api-openapi.yml
- filename: amazon-aurora-global-clusters-api-openapi.yml
  format: yaml
  label: Amazon Aurora Global Clusters API
  slug: amazon-aurora-global-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/openapi/amazon-aurora-global-clusters-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: rds.us-east-1.amazonaws.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Aurora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Aurora, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Aurora
provider_slug: amazon-aurora
slug: amazon-aurora-domain-security
source_filename: amazon-aurora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: rds.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-aurora/refs/heads/main/security/amazon-aurora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Aurora
- MySQL
- PostgreSQL
- Relational Database
---
