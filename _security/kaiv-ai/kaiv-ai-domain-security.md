---
api_specs:
- filename: kaiv-ai-account-api-openapi.yml
  format: yaml
  label: kaiv-ai Account API
  slug: kaiv-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-account-api-openapi.yml
- filename: kaiv-ai-activity-api-openapi.yml
  format: yaml
  label: kaiv-ai Activity API
  slug: kaiv-ai-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-activity-api-openapi.yml
- filename: kaiv-ai-changes-api-openapi.yml
  format: yaml
  label: kaiv-ai Changes API
  slug: kaiv-ai-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-changes-api-openapi.yml
- filename: kaiv-ai-credentials-api-openapi.yml
  format: yaml
  label: kaiv-ai Credentials API
  slug: kaiv-ai-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-credentials-api-openapi.yml
- filename: kaiv-ai-documents-api-openapi.yml
  format: yaml
  label: kaiv-ai Documents API
  slug: kaiv-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-documents-api-openapi.yml
- filename: kaiv-ai-keys-api-openapi.yml
  format: yaml
  label: kaiv-ai Keys API
  slug: kaiv-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-keys-api-openapi.yml
- filename: kaiv-ai-no-account-api-openapi.yml
  format: yaml
  label: kaiv-ai No account API
  slug: kaiv-ai-no-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-no-account-api-openapi.yml
- filename: kaiv-ai-policies-api-openapi.yml
  format: yaml
  label: kaiv-ai Policies API
  slug: kaiv-ai-policies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-policies-api-openapi.yml
- filename: kaiv-ai-servers-api-openapi.yml
  format: yaml
  label: kaiv-ai Servers API
  slug: kaiv-ai-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaiv-ai/openapi/kaiv-ai-servers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kaiv.ai
  spf: true
hosts:
- cert_expires: Dec  8 12:41:21 2026 GMT
  host: kaiv.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kaiv Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kaiv-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: kaiv-ai
provider_slug: kaiv-ai
slug: kaiv-ai-domain-security
source_filename: kaiv-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaiv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 12:41:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kaiv.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kaiv-ai/security/kaiv-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Infrastructure
- MCP
- Bridge
- Enterprise
- DeveloperTools
---
