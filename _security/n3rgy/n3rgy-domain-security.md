---
api_specs:
- filename: n3rgy-create-export-profiles-api-openapi.yml
  format: yaml
  label: n3rgy Create Export Profiles API
  slug: n3rgy-create-export-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-create-export-profiles-api-openapi.yml
- filename: n3rgy-customer-service-api-v2-api-openapi.yml
  format: yaml
  label: n3rgy Customer Service API V2 API
  slug: n3rgy-customer-service-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-customer-service-api-v2-api-openapi.yml
- filename: n3rgy-find-mpxn-api-openapi.yml
  format: yaml
  label: n3rgy Find Mpxn API
  slug: n3rgy-find-mpxn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-find-mpxn-api-openapi.yml
- filename: n3rgy-get-update-frequencies-api-openapi.yml
  format: yaml
  label: n3rgy Get Update Frequencies API
  slug: n3rgy-get-update-frequencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-get-update-frequencies-api-openapi.yml
- filename: n3rgy-internal-api-openapi.yml
  format: yaml
  label: n3rgy Internal API
  slug: n3rgy-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-internal-api-openapi.yml
- filename: n3rgy-mpxn-api-openapi.yml
  format: yaml
  label: n3rgy Mpxn API
  slug: n3rgy-mpxn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-mpxn-api-openapi.yml
- filename: n3rgy-push-api-openapi.yml
  format: yaml
  label: n3rgy Push API
  slug: n3rgy-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-push-api-openapi.yml
- filename: n3rgy-read-inventory-api-openapi.yml
  format: yaml
  label: n3rgy Read Inventory API
  slug: n3rgy-read-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-read-inventory-api-openapi.yml
- filename: n3rgy-reset-all-update-frequencies-api-openapi.yml
  format: yaml
  label: n3rgy Reset All Update Frequencies API
  slug: n3rgy-reset-all-update-frequencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-reset-all-update-frequencies-api-openapi.yml
- filename: n3rgy-set-defaults-api-openapi.yml
  format: yaml
  label: n3rgy Set Defaults API
  slug: n3rgy-set-defaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-set-defaults-api-openapi.yml
- filename: n3rgy-set-meter-update-frequency-api-openapi.yml
  format: yaml
  label: n3rgy Set Meter Update Frequency API
  slug: n3rgy-set-meter-update-frequency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-set-meter-update-frequency-api-openapi.yml
- filename: n3rgy-update-now-api-openapi.yml
  format: yaml
  label: n3rgy Update Now API
  slug: n3rgy-update-now-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-update-now-api-openapi.yml
- filename: n3rgy-upload-api-openapi.yml
  format: yaml
  label: n3rgy Upload API
  slug: n3rgy-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/openapi/n3rgy-upload-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: n3rgy.com
  spf: true
hosts:
- cert_expires: Oct 24 07:00:29 2026 GMT
  host: www.n3rgy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: data.n3rgy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: customer-api-user-manuals.data.n3rgy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: N3Rgy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for n3rgy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: n3rgy
provider_slug: n3rgy
slug: n3rgy-domain-security
source_filename: n3rgy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.n3rgy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 07:00:29 2026 GMT\n  hsts: null\n- host: data.n3rgy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customer-api-user-manuals.data.n3rgy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: n3rgy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n3rgy/refs/heads/main/security/n3rgy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Energy
- United Kingdom
- Utilities
- Smart Metering
- Electricity
- Gas
- Smart Meter Data
- Consent
- Metering
- Energy Data
---
