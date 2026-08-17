---
api_specs:
- filename: google-tag-manager-accounts-api-openapi.yml
  format: yaml
  label: Google Tag Manager Accounts API
  slug: google-tag-manager-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-accounts-api-openapi.yml
- filename: google-tag-manager-containers-api-openapi.yml
  format: yaml
  label: Google Tag Manager Containers API
  slug: google-tag-manager-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-containers-api-openapi.yml
- filename: google-tag-manager-tagmanager-api-openapi.yml
  format: yaml
  label: Google Tag Manager Tagmanager API
  slug: google-tag-manager-tagmanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-tagmanager-api-openapi.yml
- filename: google-tag-manager-triggers-api-openapi.yml
  format: yaml
  label: Google Tag Manager Triggers API
  slug: google-tag-manager-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-triggers-api-openapi.yml
- filename: google-tag-manager-user-permissions-api-openapi.yml
  format: yaml
  label: Google Tag Manager User Permissions API
  slug: google-tag-manager-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-user-permissions-api-openapi.yml
- filename: google-tag-manager-variables-api-openapi.yml
  format: yaml
  label: Google Tag Manager Variables API
  slug: google-tag-manager-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-variables-api-openapi.yml
- filename: google-tag-manager-versions-api-openapi.yml
  format: yaml
  label: Google Tag Manager Versions API
  slug: google-tag-manager-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-versions-api-openapi.yml
- filename: google-tag-manager-workspaces-api-openapi.yml
  format: yaml
  label: Google Tag Manager Workspaces API
  slug: google-tag-manager-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/openapi/google-tag-manager-workspaces-api-openapi.yml
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
- cert_expires: Oct 12 18:05:55 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 18:07:34 2026 GMT
  host: tagmanager.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Tag Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Tag Manager, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Tag Manager
provider_slug: google-tag-manager
slug: google-tag-manager-domain-security
source_filename: google-tag-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:05:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tagmanager.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 18:07:34 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/security/google-tag-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
---
