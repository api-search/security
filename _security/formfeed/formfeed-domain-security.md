---
api_specs:
- filename: formfeed-account-api-openapi.yml
  format: yaml
  label: Formfeed Account API
  slug: formfeed-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-account-api-openapi.yml
- filename: formfeed-brand-api-openapi.yml
  format: yaml
  label: Formfeed Brand API
  slug: formfeed-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-brand-api-openapi.yml
- filename: formfeed-compat-api-openapi.yml
  format: yaml
  label: Formfeed Compat API
  slug: formfeed-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-compat-api-openapi.yml
- filename: formfeed-files-api-openapi.yml
  format: yaml
  label: Formfeed Files API
  slug: formfeed-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-files-api-openapi.yml
- filename: formfeed-partials-api-openapi.yml
  format: yaml
  label: Formfeed Partials API
  slug: formfeed-partials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-partials-api-openapi.yml
- filename: formfeed-pdf-tools-api-openapi.yml
  format: yaml
  label: Formfeed PDF tools API
  slug: formfeed-pdf-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-pdf-tools-api-openapi.yml
- filename: formfeed-renders-api-openapi.yml
  format: yaml
  label: Formfeed Renders API
  slug: formfeed-renders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-renders-api-openapi.yml
- filename: formfeed-templates-api-openapi.yml
  format: yaml
  label: Formfeed Templates API
  slug: formfeed-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-templates-api-openapi.yml
- filename: formfeed-webhooks-api-openapi.yml
  format: yaml
  label: Formfeed Webhooks API
  slug: formfeed-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/openapi/formfeed-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formfeed.dev
  spf: true
hosts:
- cert_expires: Dec 16 17:39:37 2026 GMT
  host: formfeed.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 14:03:23 2026 GMT
  host: docs.formfeed.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 14:03:31 2026 GMT
  host: api.formfeed.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Formfeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formfeed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Formfeed
provider_slug: formfeed
slug: formfeed-domain-security
source_filename: formfeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formfeed.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 17:39:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.formfeed.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:03:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.formfeed.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:03:31 2026 GMT\n  hsts: null\ndomains:\n- domain: formfeed.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formfeed/refs/heads/main/security/formfeed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Image Generation
- Templates
- Developer Tools
- Software-as-a-Service
---
