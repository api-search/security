---
api_specs:
- filename: asapp-conversations-openapi.yml
  format: yaml
  label: ASAPP Conversations API
  slug: asapp-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-conversations-openapi.yml
- filename: asapp-generativeagent-openapi.yml
  format: yaml
  label: ASAPP GenerativeAgent API
  slug: asapp-generativeagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-generativeagent-openapi.yml
- filename: asapp-autosummary-openapi.yml
  format: yaml
  label: ASAPP AutoSummary API
  slug: asapp-autosummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autosummary-openapi.yml
- filename: asapp-autocompose-openapi.yml
  format: yaml
  label: ASAPP AutoCompose API
  slug: asapp-autocompose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autocompose-openapi.yml
- filename: asapp-autotranscribe-openapi.yml
  format: yaml
  label: ASAPP AutoTranscribe API
  slug: asapp-autotranscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autotranscribe-openapi.yml
- filename: asapp-knowledge-base-openapi.yml
  format: yaml
  label: ASAPP Knowledge Base API
  slug: asapp-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-knowledge-base-openapi.yml
- filename: asapp-metadata-ingestion-openapi.yml
  format: yaml
  label: ASAPP Metadata Ingestion API
  slug: asapp-metadata-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-metadata-ingestion-openapi.yml
- filename: asapp-fileexporter-openapi.yml
  format: yaml
  label: ASAPP File Exporter API
  slug: asapp-file-exporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-fileexporter-openapi.yml
- filename: asapp-partner-configuration-openapi.yml
  format: yaml
  label: ASAPP Partner Configuration API
  slug: asapp-partner-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-partner-configuration-openapi.yml
- filename: asapp-mg-genagent-openapi.yml
  format: yaml
  label: ASAPP GenAgent Media Gateway API
  slug: asapp-genagent-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-mg-genagent-openapi.yml
- filename: asapp-mg-autotranscribe-openapi.yml
  format: yaml
  label: ASAPP AutoTranscribe Media Gateway API
  slug: asapp-autotranscribe-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-mg-autotranscribe-openapi.yml
- filename: asapp-healthcheck-openapi.yml
  format: yaml
  label: ASAPP Health Check API
  slug: asapp-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-healthcheck-openapi.yml
- filename: asapp-openapi-openapi.yml
  format: yaml
  label: ASAPP Platform API (combined)
  slug: asapp-platform-api-combined
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-openapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asapp.com
  spf: true
hosts:
- cert_expires: Aug 20 16:03:38 2026 GMT
  host: www.asapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 06:12:02 2026 GMT
  host: api.sandbox.asapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 06:08:43 2026 GMT
  host: api.test.asapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASAPP, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ASAPP
provider_slug: asapp
slug: asapp-domain-security
source_filename: asapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:03:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sandbox.asapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:12:02 2026 GMT\n  hsts: null\n- host: api.test.asapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 06:08:43 2026 GMT\n  hsts: null\ndomains:\n- domain: asapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/security/asapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Conversational AI
- Contact Center
- Customer Experience
- Customer Service
- Generative AI
- Agent Assist
- Speech Recognition
- Knowledge Base
---
