---
api_specs:
- filename: githunt-ai-briefs-api-openapi.yml
  format: yaml
  label: githunt-ai Briefs API
  slug: githunt-ai-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-briefs-api-openapi.yml
- filename: githunt-ai-lists-api-openapi.yml
  format: yaml
  label: githunt-ai Lists API
  slug: githunt-ai-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-lists-api-openapi.yml
- filename: githunt-ai-profile-api-openapi.yml
  format: yaml
  label: githunt-ai Profile API
  slug: githunt-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-profile-api-openapi.yml
- filename: githunt-ai-search-api-openapi.yml
  format: yaml
  label: githunt-ai Search API
  slug: githunt-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-search-api-openapi.yml
- filename: githunt-ai-users-api-openapi.yml
  format: yaml
  label: githunt-ai Users API
  slug: githunt-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githunt-ai/openapi/githunt-ai-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: githunt.ai
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: githunt.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Githunt Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for githunt-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: githunt-ai
provider_slug: githunt-ai
slug: githunt-ai-domain-security
source_filename: githunt-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: githunt.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: githunt.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/githunt-ai/security/githunt-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Talent
- Recruitment
- Developer
---
