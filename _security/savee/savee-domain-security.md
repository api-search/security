---
api_specs:
- filename: savee-boards-api-openapi.yml
  format: yaml
  label: Savee Boards API
  slug: savee-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-boards-api-openapi.yml
- filename: savee-saves-api-openapi.yml
  format: yaml
  label: Savee Saves API
  slug: savee-saves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-saves-api-openapi.yml
- filename: savee-search-api-openapi.yml
  format: yaml
  label: Savee Search API
  slug: savee-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-search-api-openapi.yml
- filename: savee-system-api-openapi.yml
  format: yaml
  label: Savee System API
  slug: savee-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-system-api-openapi.yml
- filename: savee-user-api-openapi.yml
  format: yaml
  label: Savee User API
  slug: savee-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/openapi/savee-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savee.com
  spf: true
hosts:
- cert_expires: Nov  7 03:23:27 2026 GMT
  host: savee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:34:58 2026 GMT
  host: docs.savee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 21:51:38 2026 GMT
  host: api.savee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Savee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Savee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Savee
provider_slug: savee
slug: savee-domain-security
source_filename: savee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: savee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 03:23:27 2026 GMT\n  hsts: false\n- host: docs.savee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:34:58 2026 GMT\n  hsts: false\n- host: api.savee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:51:38 2026 GMT\n  hsts: null\ndomains:\n- domain: savee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savee/refs/heads/main/security/savee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Design
- visual inspiration
- Image
- Creative
- Moodboards
- Artificial Intelligence (AI)
---
