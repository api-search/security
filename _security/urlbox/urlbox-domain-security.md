---
api_specs:
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Synchronous Render API
  slug: urlbox-render-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Asynchronous Render API
  slug: urlbox-render-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Render Status API
  slug: urlbox-render-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Render Links API
  slug: urlbox-render-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Webhooks API
  slug: urlbox-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Usage API
  slug: urlbox-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urlbox.com
  spf: false
hosts:
- cert_expires: Sep  8 21:47:09 2026 GMT
  host: urlbox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 08:24:26 2026 GMT
  host: api.urlbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urlbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urlbox, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Urlbox
provider_slug: urlbox
slug: urlbox-domain-security
source_filename: urlbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urlbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.urlbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 08:24:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urlbox.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/security/urlbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Screenshots
- Rendering
- PDF
- Video
- Web Capture
---
