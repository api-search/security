---
api_specs:
- filename: camtasia-assets-api-openapi.yml
  format: yaml
  label: Camtasia Assets API
  slug: camtasia-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-assets-api-openapi.yml
- filename: camtasia-categories-api-openapi.yml
  format: yaml
  label: Camtasia Categories API
  slug: camtasia-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-categories-api-openapi.yml
- filename: camtasia-downloads-api-openapi.yml
  format: yaml
  label: Camtasia Downloads API
  slug: camtasia-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-downloads-api-openapi.yml
- filename: camtasia-libraries-api-openapi.yml
  format: yaml
  label: Camtasia Libraries API
  slug: camtasia-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-libraries-api-openapi.yml
- filename: camtasia-media-api-openapi.yml
  format: yaml
  label: Camtasia Media API
  slug: camtasia-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-media-api-openapi.yml
- filename: camtasia-productions-api-openapi.yml
  format: yaml
  label: Camtasia Productions API
  slug: camtasia-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-productions-api-openapi.yml
- filename: camtasia-projects-api-openapi.yml
  format: yaml
  label: Camtasia Projects API
  slug: camtasia-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-projects-api-openapi.yml
- filename: camtasia-recordings-api-openapi.yml
  format: yaml
  label: Camtasia Recordings API
  slug: camtasia-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-recordings-api-openapi.yml
- filename: camtasia-templates-api-openapi.yml
  format: yaml
  label: Camtasia Templates API
  slug: camtasia-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-templates-api-openapi.yml
- filename: camtasia-tracks-api-openapi.yml
  format: yaml
  label: Camtasia Tracks API
  slug: camtasia-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/openapi/camtasia-tracks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: techsmith.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: screencast.com
  spf: true
hosts:
- cert_expires: Sep 24 10:59:21 2026 GMT
  host: www.techsmith.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 10:59:21 2026 GMT
  host: app.screencast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 16:15:11 2026 GMT
  host: api.techsmith.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Camtasia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camtasia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Camtasia
provider_slug: camtasia
slug: camtasia-domain-security
source_filename: camtasia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.techsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:59:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.screencast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:59:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.techsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 16:15:11 2026 GMT\n  hsts: null\ndomains:\n- domain: techsmith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: screencast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/security/camtasia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
---
