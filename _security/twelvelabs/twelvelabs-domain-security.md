---
api_specs:
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Indexes API
  slug: twelvelabs-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Tasks (Upload) API
  slug: twelvelabs-tasks-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Search API
  slug: twelvelabs-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Analyze / Generate API
  slug: twelvelabs-analyze-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
- filename: twelvelabs-openapi.yml
  format: yaml
  label: TwelveLabs Embed API
  slug: twelvelabs-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/openapi/twelvelabs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: twelvelabs.io
  spf: true
hosts:
- cert_expires: Aug 20 10:27:15 2026 GMT
  host: www.twelvelabs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 18:53:04 2026 GMT
  host: docs.twelvelabs.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.twelvelabs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twelvelabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TwelveLabs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TwelveLabs
provider_slug: twelvelabs
slug: twelvelabs-domain-security
source_filename: twelvelabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twelvelabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:27:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.twelvelabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 18:53:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.twelvelabs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: twelvelabs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twelvelabs/refs/heads/main/security/twelvelabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Video Understanding
- Multimodal
- Search
- Embeddings
---
