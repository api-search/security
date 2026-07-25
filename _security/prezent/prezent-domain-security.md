---
api_specs:
- filename: prezent-audiences-api-openapi.yml
  format: yaml
  label: Prezent Audiences API
  slug: prezent-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-audiences-api-openapi.yml
- filename: prezent-autogenerator-api-openapi.yml
  format: yaml
  label: Prezent AutoGenerator API
  slug: prezent-autogenerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-autogenerator-api-openapi.yml
- filename: prezent-file-access-api-openapi.yml
  format: yaml
  label: Prezent File Access API
  slug: prezent-file-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-file-access-api-openapi.yml
- filename: prezent-health-api-openapi.yml
  format: yaml
  label: Prezent Health API
  slug: prezent-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-health-api-openapi.yml
- filename: prezent-streaming-api-openapi.yml
  format: yaml
  label: Prezent Streaming API
  slug: prezent-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-streaming-api-openapi.yml
- filename: prezent-template-converter-api-openapi.yml
  format: yaml
  label: Prezent Template Converter API
  slug: prezent-template-converter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-template-converter-api-openapi.yml
- filename: prezent-themes-api-openapi.yml
  format: yaml
  label: Prezent Themes API
  slug: prezent-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-themes-api-openapi.yml
- filename: prezent-upload-api-openapi.yml
  format: yaml
  label: Prezent Upload API
  slug: prezent-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-upload-api-openapi.yml
- filename: prezent-webhooks-api-openapi.yml
  format: yaml
  label: Prezent Webhooks API
  slug: prezent-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/openapi/prezent-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prezent.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: myprezent.com
  spf: false
hosts:
- cert_expires: Oct  6 00:09:14 2026 GMT
  host: prezent.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.prezent.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: uatstage-api.myprezent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prezent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prezent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prezent
provider_slug: prezent
slug: prezent-domain-security
source_filename: prezent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prezent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:09:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prezent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: uatstage-api.myprezent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: prezent.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: myprezent.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prezent/refs/heads/main/security/prezent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Presentations
- Generative AI
- AI Agents
- Life Sciences
- Content Generation
- Enterprise
- MCP
- Productivity
---
