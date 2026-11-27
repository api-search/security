---
api_specs:
- filename: makeaivideo-ai-auth-api-openapi.yml
  format: yaml
  label: MakeAIVideo Auth API
  slug: makeaivideo-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-auth-api-openapi.yml
- filename: makeaivideo-ai-brand-kit-api-openapi.yml
  format: yaml
  label: MakeAIVideo Brand kit API
  slug: makeaivideo-ai-brand-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-brand-kit-api-openapi.yml
- filename: makeaivideo-ai-characters-api-openapi.yml
  format: yaml
  label: MakeAIVideo Characters API
  slug: makeaivideo-ai-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-characters-api-openapi.yml
- filename: makeaivideo-ai-ideas-api-openapi.yml
  format: yaml
  label: MakeAIVideo Ideas API
  slug: makeaivideo-ai-ideas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-ideas-api-openapi.yml
- filename: makeaivideo-ai-introspection-api-openapi.yml
  format: yaml
  label: MakeAIVideo Introspection API
  slug: makeaivideo-ai-introspection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-introspection-api-openapi.yml
- filename: makeaivideo-ai-music-api-openapi.yml
  format: yaml
  label: MakeAIVideo Music API
  slug: makeaivideo-ai-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-music-api-openapi.yml
- filename: makeaivideo-ai-publishing-api-openapi.yml
  format: yaml
  label: MakeAIVideo Publishing API
  slug: makeaivideo-ai-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-publishing-api-openapi.yml
- filename: makeaivideo-ai-scripts-api-openapi.yml
  format: yaml
  label: MakeAIVideo Scripts API
  slug: makeaivideo-ai-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-scripts-api-openapi.yml
- filename: makeaivideo-ai-uploads-api-openapi.yml
  format: yaml
  label: MakeAIVideo Uploads API
  slug: makeaivideo-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-uploads-api-openapi.yml
- filename: makeaivideo-ai-videos-api-openapi.yml
  format: yaml
  label: MakeAIVideo Videos API
  slug: makeaivideo-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-videos-api-openapi.yml
- filename: makeaivideo-ai-voices-api-openapi.yml
  format: yaml
  label: MakeAIVideo Voices API
  slug: makeaivideo-ai-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-voices-api-openapi.yml
- filename: makeaivideo-ai-webhooks-api-openapi.yml
  format: yaml
  label: MakeAIVideo Webhooks API
  slug: makeaivideo-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-webhooks-api-openapi.yml
- filename: makeaivideo-ai-workspace-api-openapi.yml
  format: yaml
  label: MakeAIVideo Workspace API
  slug: makeaivideo-ai-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makeaivideo-ai/openapi/makeaivideo-ai-workspace-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: makeaivideo.ai
  spf: true
hosts:
- cert_expires: Feb  5 17:54:36 2027 GMT
  host: makeaivideo.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MakeAIVideo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MakeAIVideo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MakeAIVideo
provider_slug: makeaivideo-ai
slug: makeaivideo-ai-domain-security
source_filename: makeaivideo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makeaivideo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 17:54:36 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: makeaivideo.ai\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/makeaivideo-ai/security/makeaivideo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Video Generation
- Social Media Content
- Advertising
- Developer API
---
