---
api_specs:
- filename: fullstory-server-api-openapi.yml
  format: yaml
  label: FullStory Server API
  slug: fullstory-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-server-api-openapi.yml
- filename: fullstory-sessions-api-openapi.yml
  format: yaml
  label: FullStory Sessions API
  slug: fullstory-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-sessions-api-openapi.yml
- filename: fullstory-segments-export-api-openapi.yml
  format: yaml
  label: FullStory Segments Export API
  slug: fullstory-segments-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-segments-export-api-openapi.yml
- filename: fullstory-webhooks-api-openapi.yml
  format: yaml
  label: FullStory Webhooks API
  slug: fullstory-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/openapi/fullstory-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fullstory.com
  spf: true
hosts:
- cert_expires: Sep 15 19:04:01 2026 GMT
  host: www.fullstory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 04:40:54 2026 GMT
  host: developer.fullstory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:26:09 2026 GMT
  host: api.fullstory.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fullstory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FullStory, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FullStory
provider_slug: fullstory
slug: fullstory-domain-security
source_filename: fullstory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fullstory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:04:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.fullstory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:40:54 2026 GMT\n  hsts: false\n- host: api.fullstory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:26:09 2026 GMT\n  hsts: null\ndomains:\n- domain: fullstory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/security/fullstory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Session Replay
- Product Analytics
- Digital Experience
- Behavioral Analytics
- Frontend Monitoring
---
