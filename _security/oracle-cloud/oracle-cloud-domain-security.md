---
api_specs:
- filename: oracle-cloud-compute-openapi.yaml
  format: yaml
  label: Compute API
  slug: compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-compute-openapi.yaml
- filename: oracle-cloud-object-storage-openapi.yaml
  format: yaml
  label: Object Storage API
  slug: object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-object-storage-openapi.yaml
- filename: oracle-cloud-networking-openapi.yaml
  format: yaml
  label: Networking API
  slug: networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-networking-openapi.yaml
- filename: oracle-cloud-database-openapi.yaml
  format: yaml
  label: Database API
  slug: database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-database-openapi.yaml
- filename: oracle-cloud-iam-openapi.yaml
  format: yaml
  label: Identity and Access Management API
  slug: identity-and-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-iam-openapi.yaml
- filename: oracle-cloud-oke-openapi.yaml
  format: yaml
  label: Container Engine for Kubernetes API
  slug: container-engine-for-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-oke-openapi.yaml
- filename: oracle-cloud-functions-openapi.yaml
  format: yaml
  label: Functions API
  slug: functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-functions-openapi.yaml
- filename: oracle-cloud-monitoring-openapi.yaml
  format: yaml
  label: Monitoring API
  slug: monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/openapi/oracle-cloud-monitoring-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: cloud.oracle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Cloud Infrastructure, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
slug: oracle-cloud-domain-security
source_filename: oracle-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/security/oracle-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
---
