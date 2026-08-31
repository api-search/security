---
api_specs:
- filename: respondology-comment-results-api-openapi.yml
  format: yaml
  label: Respondology Comment Results API
  slug: respondology-comment-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-comment-results-api-openapi.yml
- filename: respondology-comments-api-openapi.yml
  format: yaml
  label: Respondology Comments API
  slug: respondology-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-comments-api-openapi.yml
- filename: respondology-moderation-reasons-api-openapi.yml
  format: yaml
  label: Respondology Moderation Reasons API
  slug: respondology-moderation-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-moderation-reasons-api-openapi.yml
- filename: respondology-post-results-api-openapi.yml
  format: yaml
  label: Respondology Post Results API
  slug: respondology-post-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-post-results-api-openapi.yml
- filename: respondology-posts-api-openapi.yml
  format: yaml
  label: Respondology Posts API
  slug: respondology-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/openapi/respondology-posts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: respondology.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: respondology.io
  spf: true
hosts:
- cert_expires: Oct 20 03:50:55 2026 GMT
  host: respondology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: webhooks.respondology.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Respondology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Respondology, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Respondology
provider_slug: respondology
slug: respondology-domain-security
source_filename: respondology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: respondology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 03:50:55 2026 GMT\n  hsts: false\n- host: webhooks.respondology.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: respondology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: respondology.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respondology/refs/heads/main/security/respondology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Content Moderation
- Social-Media
- Comment Moderation
- Trust and Safety
- Artificial Intelligence
- Brand Protection
- Social Listening
- Webhook
- Marketing
---
