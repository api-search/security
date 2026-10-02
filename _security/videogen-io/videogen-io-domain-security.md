---
api_specs:
- filename: videogen-io-account-api-openapi.yml
  format: yaml
  label: VideoGen Account API
  slug: videogen-io-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-account-api-openapi.yml
- filename: videogen-io-assistant-api-openapi.yml
  format: yaml
  label: VideoGen Assistant API
  slug: videogen-io-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-assistant-api-openapi.yml
- filename: videogen-io-entities-api-openapi.yml
  format: yaml
  label: VideoGen Entities API
  slug: videogen-io-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-entities-api-openapi.yml
- filename: videogen-io-files-api-openapi.yml
  format: yaml
  label: VideoGen Files API
  slug: videogen-io-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-files-api-openapi.yml
- filename: videogen-io-projects-api-openapi.yml
  format: yaml
  label: VideoGen Projects API
  slug: videogen-io-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-projects-api-openapi.yml
- filename: videogen-io-resources-api-openapi.yml
  format: yaml
  label: VideoGen Resources API
  slug: videogen-io-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-resources-api-openapi.yml
- filename: videogen-io-text-api-openapi.yml
  format: yaml
  label: VideoGen Text API
  slug: videogen-io-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-text-api-openapi.yml
- filename: videogen-io-tools-api-openapi.yml
  format: yaml
  label: VideoGen Tools API
  slug: videogen-io-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-tools-api-openapi.yml
- filename: videogen-io-webhook-events-api-openapi.yml
  format: yaml
  label: VideoGen Webhook events API
  slug: videogen-io-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-webhook-events-api-openapi.yml
- filename: videogen-io-webhooks-api-openapi.yml
  format: yaml
  label: VideoGen Webhooks API
  slug: videogen-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-webhooks-api-openapi.yml
- filename: videogen-io-workflows-api-openapi.yml
  format: yaml
  label: VideoGen Workflows API
  slug: videogen-io-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: videogen.io
  spf: true
hosts:
- cert_expires: Dec 21 00:31:14 2026 GMT
  host: videogen.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Videogen Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VideoGen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VideoGen
provider_slug: videogen-io
slug: videogen-io-domain-security
source_filename: videogen-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: videogen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 00:31:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: videogen.io\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/security/videogen-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Video
- Automation
- Platform
---
