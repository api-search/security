---
api_specs:
- filename: google-cloud-logging-bucket-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Bucket API
  slug: google-cloud-logging-bucket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-bucket-api-openapi.yml
- filename: google-cloud-logging-buckets-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Buckets API
  slug: google-cloud-logging-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-buckets-api-openapi.yml
- filename: google-cloud-logging-entries-copy-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:copy API
  slug: google-cloud-logging-entries-copy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-copy-api-openapi.yml
- filename: google-cloud-logging-entries-list-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:list API
  slug: google-cloud-logging-entries-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-list-api-openapi.yml
- filename: google-cloud-logging-entries-tail-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:tail API
  slug: google-cloud-logging-entries-tail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-tail-api-openapi.yml
- filename: google-cloud-logging-entries-write-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Entries:write API
  slug: google-cloud-logging-entries-write-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-entries-write-api-openapi.yml
- filename: google-cloud-logging-exclusions-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Exclusions API
  slug: google-cloud-logging-exclusions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-exclusions-api-openapi.yml
- filename: google-cloud-logging-google-cloud-logging-api-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Google Cloud Logging API API
  slug: google-cloud-logging-google-cloud-logging-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-google-cloud-logging-api-api-openapi.yml
- filename: google-cloud-logging-sinks-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Sinks API
  slug: google-cloud-logging-sinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/openapi/google-cloud-logging-sinks-api-openapi.yml
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
- cert_expires: Sep 14 08:41:22 2026 GMT
  host: logging.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Cloud Logging Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Logging, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Logging
provider_slug: google-cloud-logging
slug: google-cloud-logging-domain-security
source_filename: google-cloud-logging-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: logging.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:41:22 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-logging/refs/heads/main/security/google-cloud-logging-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Logging
- Monitoring
- Observability
---
