---
api_specs:
- filename: pingcap-tidb-cloud-starter-essential-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Starter and Essential API (v1beta1)
  slug: tidb-cloud-starter-and-essential-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-starter-essential-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-dedicated-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Dedicated API (v1beta1)
  slug: tidb-cloud-dedicated-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-dedicated-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-iam-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud IAM API (v1beta1)
  slug: tidb-cloud-iam-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-iam-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-billing-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Billing API (v1beta1)
  slug: tidb-cloud-billing-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-billing-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Data Service API (v1beta1)
  slug: tidb-cloud-data-service-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-v1beta-openapi-original.json
  format: json
  label: TiDB Cloud API (v1beta, legacy)
  slug: tidb-cloud-api-v1beta-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-v1beta-openapi-original.json
- filename: pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json
  format: json
  label: TiDB Cloud Zero API (v1alpha1)
  slug: tidb-cloud-zero-api-v1alpha1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json
- filename: pingcap-tidb-dm-openapi-original.yaml
  format: yaml
  label: TiDB Data Migration (DM) OpenAPI
  slug: tidb-data-migration-dm-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-dm-openapi-original.yaml
- filename: pingcap-ossinsight-public-api-openapi-original.yaml
  format: yaml
  label: OSS Insight Public API
  slug: oss-insight-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-ossinsight-public-api-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pingcap.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tidbapi.com
  spf: false
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.pingcap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: docs.pingcap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: serverless.tidbapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pingcap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PingCAP, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PingCAP
provider_slug: pingcap
slug: pingcap-domain-security
source_filename: pingcap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pingcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pingcap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: false\n- host: serverless.tidbapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pingcap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tidbapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/security/pingcap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- distributed-sql
- database
- tidb
- htap
- mysql-compatible
- cloud-database
- dbaas
- vector-search
- data-migration
- change-data-capture
- open-source
- infrastructure
---
