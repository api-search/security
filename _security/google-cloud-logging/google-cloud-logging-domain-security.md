---
api_specs:
- filename: google-cloud-logging-exclusions-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Exclusions API
  slug: google-cloud-logging-exclusions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-exclusions-api-openapi.yml
- filename: google-cloud-logging-sinks-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Sinks API
  slug: google-cloud-logging-sinks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-sinks-api-openapi.yml
- filename: google-cloud-logging-entries-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cloud Logging Entries API
  slug: google-cloud-logging-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-entries-api-openapi.yml
- filename: google-cloud-logging-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cloud Logging Folders API
  slug: google-cloud-logging-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-folders-api-openapi.yml
- filename: google-cloud-logging-locations-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cloud Logging Locations API
  slug: google-cloud-logging-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-locations-api-openapi.yml
- filename: google-cloud-logging-logs-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cloud Logging Logs API
  slug: google-cloud-logging-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-logs-api-openapi.yml
- filename: google-cloud-logging-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cloud Logging Organizations API
  slug: google-cloud-logging-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-organizations-api-openapi.yml
- filename: google-cloud-logging-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cloud Logging Projects API
  slug: google-cloud-logging-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-projects-api-openapi.yml
- filename: google-cloud-logging-billingaccounts-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Billing Accounts API
  slug: google-cloud-logging-billingaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-billingaccounts-api-openapi.yml
- filename: google-cloud-logging-cmeksettings-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Cmek Settings API
  slug: google-cloud-logging-cmeksettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-cmeksettings-api-openapi.yml
- filename: google-cloud-logging-monitoredresourcedescriptors-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Monitored Resource Descriptors API
  slug: google-cloud-logging-monitoredresourcedescriptors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-monitoredresourcedescriptors-api-openapi.yml
- filename: google-cloud-logging-settings-api-openapi.yml
  format: yaml
  label: Google Cloud Logging Settings API
  slug: google-cloud-logging-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-logging/openapi/google-cloud-logging-settings-api-openapi.yml
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
- cert_expires: Nov  2 08:38:57 2026 GMT
  host: console.cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:37:34 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 08:41:51 2026 GMT
  host: logging.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
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
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:38:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:37:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: logging.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 08:41:51 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-logging/security/google-cloud-logging-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Logging
- Monitoring
- Observability
- Telemetry
- Log Management
- SRE
- DevOps
- OpenTelemetry
- Google Cloud
---
