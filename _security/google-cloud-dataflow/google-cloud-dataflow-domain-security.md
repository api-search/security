---
api_specs:
- filename: google-cloud-dataflow-debug-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Debug API
  slug: google-cloud-dataflow-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-debug-api-openapi.yml
- filename: google-cloud-dataflow-flex-templates-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Flex Templates API
  slug: google-cloud-dataflow-flex-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-flex-templates-api-openapi.yml
- filename: google-cloud-dataflow-jobs-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Jobs API
  slug: google-cloud-dataflow-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-jobs-api-openapi.yml
- filename: google-cloud-dataflow-messages-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Messages API
  slug: google-cloud-dataflow-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-messages-api-openapi.yml
- filename: google-cloud-dataflow-metrics-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Metrics API
  slug: google-cloud-dataflow-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-metrics-api-openapi.yml
- filename: google-cloud-dataflow-snapshots-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Snapshots API
  slug: google-cloud-dataflow-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-snapshots-api-openapi.yml
- filename: google-cloud-dataflow-stages-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Stages API
  slug: google-cloud-dataflow-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-stages-api-openapi.yml
- filename: google-cloud-dataflow-templates-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Templates API
  slug: google-cloud-dataflow-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/openapi/google-cloud-dataflow-templates-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:41:22 2026 GMT
  host: dataflow.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Cloud Dataflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Dataflow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
slug: google-cloud-dataflow-domain-security
source_filename: google-cloud-dataflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dataflow.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:41:22 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/security/google-cloud-dataflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
---
