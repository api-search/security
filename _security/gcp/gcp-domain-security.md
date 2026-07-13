---
api_specs:
- filename: rest
  format: yaml
  label: Compute Engine API
  slug: compute-engine
  spec_type: OpenAPI
  url: https://compute.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Storage API
  slug: cloud-storage
  spec_type: OpenAPI
  url: https://storage.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Functions API
  slug: cloud-functions
  spec_type: OpenAPI
  url: https://cloudfunctions.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Pub/Sub API
  slug: cloud-pubsub
  spec_type: OpenAPI
  url: https://pubsub.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: BigQuery API
  slug: bigquery
  spec_type: OpenAPI
  url: https://bigquery.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Cloud Vision API
  slug: cloud-vision
  spec_type: OpenAPI
  url: https://vision.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Natural Language API
  slug: cloud-natural-language
  spec_type: OpenAPI
  url: https://language.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Kubernetes Engine API
  slug: kubernetes-engine
  spec_type: OpenAPI
  url: https://container.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud SQL Admin API
  slug: cloud-sql
  spec_type: OpenAPI
  url: https://sqladmin.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Cloud Firestore API
  slug: cloud-firestore
  spec_type: OpenAPI
  url: https://firestore.googleapis.com/$discovery/rest?version=v1
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
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: compute.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:41:23 2026 GMT
  host: storage.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Platform APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Platform APIs
provider_slug: gcp
slug: gcp-domain-security
source_filename: gcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: compute.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: storage.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:41:23 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gcp/refs/heads/main/security/gcp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Databases
- Infrastructure
- Machine Learning
- Networking
- Security
- Serverless
- Storage
---
