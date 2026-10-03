---
api_specs:
- filename: asapp3-autocompose-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Compose API
  slug: asapp3-autocompose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autocompose-api-openapi.yml
- filename: asapp3-autosummary-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Summary API
  slug: asapp3-autosummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autosummary-api-openapi.yml
- filename: asapp3-autotranscribe-api-openapi.yml
  format: yaml
  label: Asapp3 Auto Transcribe API
  slug: asapp3-autotranscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autotranscribe-api-openapi.yml
- filename: asapp3-autotranscribe-media-gateway-api-openapi.yml
  format: yaml
  label: Asapp3 AutoTranscribe Media Gateway API
  slug: asapp3-autotranscribe-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-autotranscribe-media-gateway-api-openapi.yml
- filename: asapp3-conversations-api-openapi.yml
  format: yaml
  label: Asapp3 Conversations API
  slug: asapp3-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-conversations-api-openapi.yml
- filename: asapp3-file-exporter-api-openapi.yml
  format: yaml
  label: Asapp3 File Exporter API
  slug: asapp3-file-exporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-file-exporter-api-openapi.yml
- filename: asapp3-generativeagent-api-openapi.yml
  format: yaml
  label: Asapp3 Generative Agent API
  slug: asapp3-generativeagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-generativeagent-api-openapi.yml
- filename: asapp3-health-check-api-openapi.yml
  format: yaml
  label: Asapp3 Health Check API
  slug: asapp3-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-health-check-api-openapi.yml
- filename: asapp3-knowledge-base-api-openapi.yml
  format: yaml
  label: Asapp3 Knowledge Base API
  slug: asapp3-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-knowledge-base-api-openapi.yml
- filename: asapp3-metadata-api-openapi.yml
  format: yaml
  label: Asapp3 Metadata API
  slug: asapp3-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/openapi/asapp3-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asapp.com
  spf: true
hosts:
- cert_expires: Dec 16 17:32:08 2026 GMT
  host: www.asapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asapp3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asapp3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Asapp3
provider_slug: asapp3
slug: asapp3-domain-security
source_filename: asapp3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 17:32:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapp3/refs/heads/main/security/asapp3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Customer Experience
- Enterprise
- Contact Center
- Platform
- Company
---
