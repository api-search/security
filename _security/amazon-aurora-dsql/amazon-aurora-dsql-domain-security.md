---
api_specs:
- filename: amazon-aurora-dsql-clusters-api-openapi.yml
  format: yaml
  label: Amazon Aurora DSQL Clusters API
  slug: amazon-aurora-dsql-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-aurora-dsql/openapi/amazon-aurora-dsql-clusters-api-openapi.yml
- filename: amazon-aurora-dsql-operations-api-openapi.yml
  format: yaml
  label: Amazon Aurora DSQL Aurora Dsql Operations API
  slug: amazon-aurora-dsql-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-aurora-dsql/openapi/amazon-aurora-dsql-operations-api-openapi.yml
- filename: amazon-aurora-dsql-policy-api-openapi.yml
  format: yaml
  label: Amazon Aurora DSQL Aurora Dsql Policy API
  slug: amazon-aurora-dsql-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-aurora-dsql/openapi/amazon-aurora-dsql-policy-api-openapi.yml
- filename: amazon-aurora-dsql-stream-api-openapi.yml
  format: yaml
  label: Amazon Aurora DSQL Aurora Dsql Stream API
  slug: amazon-aurora-dsql-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-aurora-dsql/openapi/amazon-aurora-dsql-stream-api-openapi.yml
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
- host: dsql.us-east-1.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Aurora Dsql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Aurora DSQL, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Aurora DSQL
provider_slug: amazon-aurora-dsql
slug: amazon-aurora-dsql-domain-security
source_filename: amazon-aurora-dsql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: dsql.us-east-1.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-aurora-dsql/security/amazon-aurora-dsql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Aurora DSQL
- Distributed SQL
- PostgreSQL
- Serverless
---
