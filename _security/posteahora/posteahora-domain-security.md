---
api_specs:
- filename: posteahora-accounts-api-openapi.yml
  format: yaml
  label: PosteAhora Accounts API
  slug: posteahora-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-accounts-api-openapi.yml
- filename: posteahora-analytics-api-openapi.yml
  format: yaml
  label: PosteAhora Analytics API
  slug: posteahora-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-analytics-api-openapi.yml
- filename: posteahora-ideas-api-openapi.yml
  format: yaml
  label: PosteAhora Ideas API
  slug: posteahora-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-ideas-api-openapi.yml
- filename: posteahora-media-api-openapi.yml
  format: yaml
  label: PosteAhora Media API
  slug: posteahora-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-media-api-openapi.yml
- filename: posteahora-posts-api-openapi.yml
  format: yaml
  label: PosteAhora Posts API
  slug: posteahora-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-posts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: posteahora.com
  spf: true
hosts:
- cert_expires: Dec  7 11:08:16 2026 GMT
  host: posteahora.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Posteahora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PosteAhora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PosteAhora
provider_slug: posteahora
slug: posteahora-domain-security
source_filename: posteahora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: posteahora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 11:08:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: posteahora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/security/posteahora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media
- AI Automation
- Marketing
- Software-as-a-Service
---
