---
api_specs:
- filename: lilt-create-api-openapi.yml
  format: yaml
  label: Lilt Create API
  slug: lilt-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-create-api-openapi.yml
- filename: lilt-documents-api-openapi.yml
  format: yaml
  label: Lilt Documents API
  slug: lilt-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-documents-api-openapi.yml
- filename: lilt-domains-api-openapi.yml
  format: yaml
  label: Lilt Domains API
  slug: lilt-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-domains-api-openapi.yml
- filename: lilt-files-api-openapi.yml
  format: yaml
  label: Lilt Files API
  slug: lilt-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-files-api-openapi.yml
- filename: lilt-jobs-api-openapi.yml
  format: yaml
  label: Lilt Jobs API
  slug: lilt-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-jobs-api-openapi.yml
- filename: lilt-languages-api-openapi.yml
  format: yaml
  label: Lilt Languages API
  slug: lilt-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-languages-api-openapi.yml
- filename: lilt-memories-api-openapi.yml
  format: yaml
  label: Lilt Memories API
  slug: lilt-memories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-memories-api-openapi.yml
- filename: lilt-projects-api-openapi.yml
  format: yaml
  label: Lilt Projects API
  slug: lilt-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-projects-api-openapi.yml
- filename: lilt-segments-api-openapi.yml
  format: yaml
  label: Lilt Segments API
  slug: lilt-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-segments-api-openapi.yml
- filename: lilt-translate-api-openapi.yml
  format: yaml
  label: Lilt Translate API
  slug: lilt-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-translate-api-openapi.yml
- filename: lilt-uploads-api-openapi.yml
  format: yaml
  label: Lilt Uploads API
  slug: lilt-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-uploads-api-openapi.yml
- filename: lilt-webhook-configuration-api-openapi.yml
  format: yaml
  label: Lilt Webhook Configuration API
  slug: lilt-webhook-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-webhook-configuration-api-openapi.yml
- filename: lilt-workflows-api-openapi.yml
  format: yaml
  label: Lilt Workflows API
  slug: lilt-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/openapi/lilt-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lilt.com
  spf: true
hosts:
- cert_expires: Oct 11 00:29:47 2026 GMT
  host: lilt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 11:26:37 2026 GMT
  host: support.lilt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 17:19:34 2026 GMT
  host: api.lilt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lilt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lilt
provider_slug: lilt
slug: lilt-domain-security
source_filename: lilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 00:29:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.lilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:26:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.lilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:19:34 2026 GMT\n  hsts: null\ndomains:\n- domain: lilt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilt/refs/heads/main/security/lilt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Translation
- Localization
- Machine Translation
- Language
- Content
- Translation Memory
- Agents
---
