---
api_specs:
- filename: ausca-com-agent-inboxes-api-openapi.yml
  format: yaml
  label: Ausca Agent Inboxes API
  slug: ausca-com-agent-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-agent-inboxes-api-openapi.yml
- filename: ausca-com-analyze-document-api-openapi.yml
  format: yaml
  label: Ausca Analyze Document API
  slug: ausca-com-analyze-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-analyze-document-api-openapi.yml
- filename: ausca-com-artifacts-api-openapi.yml
  format: yaml
  label: Ausca Artifacts API
  slug: ausca-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-artifacts-api-openapi.yml
- filename: ausca-com-browser-sessions-api-openapi.yml
  format: yaml
  label: Ausca Browser Sessions API
  slug: ausca-com-browser-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-browser-sessions-api-openapi.yml
- filename: ausca-com-extend-inbox-api-openapi.yml
  format: yaml
  label: Ausca Extend Inbox API
  slug: ausca-com-extend-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-extend-inbox-api-openapi.yml
- filename: ausca-com-extract-text-api-openapi.yml
  format: yaml
  label: Ausca Extract Text API
  slug: ausca-com-extract-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-extract-text-api-openapi.yml
- filename: ausca-com-invocations-api-openapi.yml
  format: yaml
  label: Ausca Invocations API
  slug: ausca-com-invocations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-invocations-api-openapi.yml
- filename: ausca-com-lease-browser-api-openapi.yml
  format: yaml
  label: Ausca Lease Browser API
  slug: ausca-com-lease-browser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-lease-browser-api-openapi.yml
- filename: ausca-com-offers-api-openapi.yml
  format: yaml
  label: Ausca Offers API
  slug: ausca-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-offers-api-openapi.yml
- filename: ausca-com-open-inbox-api-openapi.yml
  format: yaml
  label: Ausca Open Inbox API
  slug: ausca-com-open-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-open-inbox-api-openapi.yml
- filename: ausca-com-transcribe-media-api-openapi.yml
  format: yaml
  label: Ausca Transcribe Media API
  slug: ausca-com-transcribe-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ausca-com/openapi/ausca-com-transcribe-media-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ausca.com
  spf: true
hosts:
- cert_expires: Jan 28 10:08:08 2027 GMT
  host: ausca.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ausca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ausca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ausca
provider_slug: ausca-com
slug: ausca-com-domain-security
source_filename: ausca-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ausca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:08:08 2027 GMT\n  hsts: false\ndomains:\n- domain: ausca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ausca-com/security/ausca-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pay-per-call APIs
- Agent Infrastructure
- Document OCR
- Media transcription
- Inbox verification
---
