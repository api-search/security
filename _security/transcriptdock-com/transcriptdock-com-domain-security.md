---
api_specs:
- filename: transcriptdock-com-app-api-openapi.yml
  format: yaml
  label: transcriptdock-com App API
  slug: transcriptdock-com-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-app-api-openapi.yml
- filename: transcriptdock-com-batches-api-openapi.yml
  format: yaml
  label: transcriptdock-com Batches API
  slug: transcriptdock-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-batches-api-openapi.yml
- filename: transcriptdock-com-capabilities-api-openapi.yml
  format: yaml
  label: transcriptdock-com Capabilities API
  slug: transcriptdock-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-capabilities-api-openapi.yml
- filename: transcriptdock-com-jobs-api-openapi.yml
  format: yaml
  label: transcriptdock-com Jobs API
  slug: transcriptdock-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-jobs-api-openapi.yml
- filename: transcriptdock-com-language-discoveries-api-openapi.yml
  format: yaml
  label: transcriptdock-com Language Discoveries API
  slug: transcriptdock-com-language-discoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-language-discoveries-api-openapi.yml
- filename: transcriptdock-com-llms-api-openapi.yml
  format: yaml
  label: transcriptdock-com Llms API
  slug: transcriptdock-com-llms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-llms-api-openapi.yml
- filename: transcriptdock-com-llms-full-api-openapi.yml
  format: yaml
  label: transcriptdock-com Llms Full API
  slug: transcriptdock-com-llms-full-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-llms-full-api-openapi.yml
- filename: transcriptdock-com-transcripts-api-openapi.yml
  format: yaml
  label: transcriptdock-com Transcripts API
  slug: transcriptdock-com-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-transcripts-api-openapi.yml
- filename: transcriptdock-com-uploads-api-openapi.yml
  format: yaml
  label: transcriptdock-com Uploads API
  slug: transcriptdock-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-uploads-api-openapi.yml
- filename: transcriptdock-com-usage-api-openapi.yml
  format: yaml
  label: transcriptdock-com Usage API
  slug: transcriptdock-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-usage-api-openapi.yml
- filename: transcriptdock-com-video-discoveries-api-openapi.yml
  format: yaml
  label: transcriptdock-com Video Discoveries API
  slug: transcriptdock-com-video-discoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-video-discoveries-api-openapi.yml
- filename: transcriptdock-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: transcriptdock-com Webhook Endpoints API
  slug: transcriptdock-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-webhook-endpoints-api-openapi.yml
- filename: transcriptdock-com-webhooks-api-openapi.yml
  format: yaml
  label: transcriptdock-com Webhooks API
  slug: transcriptdock-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/transcriptdock-com/openapi/transcriptdock-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: transcriptdock.com
  spf: true
hosts:
- cert_expires: Dec 30 20:23:55 2026 GMT
  host: transcriptdock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Transcriptdock Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for transcriptdock-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: transcriptdock-com
provider_slug: transcriptdock-com
slug: transcriptdock-com-domain-security
source_filename: transcriptdock-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcriptdock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 20:23:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transcriptdock.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/transcriptdock-com/security/transcriptdock-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video
- Transcript
- API
- YouTube
- TikTok
---
