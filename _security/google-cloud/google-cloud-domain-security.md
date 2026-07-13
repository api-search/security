---
api_specs:
- filename: rest
  format: yaml
  label: Google Compute Engine API
  slug: google-compute-engine-api
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Storage API
  slug: google-cloud-storage-api
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Kubernetes Engine API
  slug: google-kubernetes-engine-api
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Functions API
  slug: google-cloud-functions-api
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google BigQuery API
  slug: google-bigquery-api
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Google Cloud Pub/Sub API
  slug: google-cloud-pubsub-api
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud Vision API
  slug: google-cloud-vision-api
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Cloud SQL Admin API
  slug: google-cloud-sql-admin-api
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
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
- cert_expires: Sep 14 08:37:10 2026 GMT
  host: console.cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: compute.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Platform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Platform
provider_slug: google-cloud
slug: google-cloud-domain-security
source_filename: google-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: compute.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud/refs/heads/main/security/google-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Data Analytics
- Infrastructure
- Machine Learning
- Platform as a Service
---
