---
api_specs:
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Media Upload API
  slug: blotato-media-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Posts Publishing API
  slug: blotato-posts-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato AI Content API
  slug: blotato-ai-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
- filename: blotato-openapi.yml
  format: yaml
  label: Blotato Accounts API
  slug: blotato-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/openapi/blotato-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blotato.com
  spf: true
hosts:
- cert_expires: Sep 29 20:37:25 2026 GMT
  host: www.blotato.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:03:28 2026 GMT
  host: help.blotato.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:21:30 2026 GMT
  host: backend.blotato.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blotato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blotato, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blotato
provider_slug: blotato
slug: blotato-domain-security
source_filename: blotato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blotato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:37:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.blotato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:03:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: backend.blotato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:21:30 2026 GMT\n  hsts: null\ndomains:\n- domain: blotato.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blotato/refs/heads/main/security/blotato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Publishing
- AI Content
- Automation
- Content Creation
---
