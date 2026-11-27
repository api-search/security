---
api_specs:
- filename: google-cloud-dataflow-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Folders API
  slug: google-cloud-dataflow-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dataflow/openapi/google-cloud-dataflow-folders-api-openapi.yml
- filename: google-cloud-dataflow-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Organizations API
  slug: google-cloud-dataflow-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dataflow/openapi/google-cloud-dataflow-organizations-api-openapi.yml
- filename: google-cloud-dataflow-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Dataflow Projects API
  slug: google-cloud-dataflow-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-dataflow/openapi/google-cloud-dataflow-projects-api-openapi.yml
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
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:11:53 2026 GMT
  host: dataflow.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: datapipelines.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Cloud Dataflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Dataflow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
slug: google-cloud-dataflow-domain-security
source_filename: google-cloud-dataflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dataflow.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:11:53 2026 GMT\n  hsts: null\n- host: datapipelines.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-dataflow/security/google-cloud-dataflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
---
