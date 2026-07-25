---
api_specs:
- filename: google-cloud-platform-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Folders API
  slug: google-cloud-platform-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-folders-api-openapi.yml
- filename: google-cloud-platform-operations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Operations API
  slug: google-cloud-platform-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-operations-api-openapi.yml
- filename: google-cloud-platform-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Organizations API
  slug: google-cloud-platform-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-organizations-api-openapi.yml
- filename: google-cloud-platform-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Platform Projects API
  slug: google-cloud-platform-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-projects-api-openapi.yml
- filename: google-cloud-platform-tagbindings-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagBindings API
  slug: google-cloud-platform-tagbindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagbindings-api-openapi.yml
- filename: google-cloud-platform-tagkeys-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagKeys API
  slug: google-cloud-platform-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagkeys-api-openapi.yml
- filename: google-cloud-platform-tagvalues-api-openapi.yml
  format: yaml
  label: Google Cloud Platform TagValues API
  slug: google-cloud-platform-tagvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/openapi/google-cloud-platform-tagvalues-api-openapi.yml
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
name: Google Cloud Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Cloud Platform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
slug: google-cloud-platform-domain-security
source_filename: google-cloud-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: compute.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\n- host: storage.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:41:23 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/security/google-cloud-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
---
