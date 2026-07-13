---
api_specs:
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy API Registry (Artifacts) API
  slug: speakeasy-api-registry-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Workspaces API
  slug: speakeasy-api-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Organizations API
  slug: speakeasy-api-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Schema Store API
  slug: speakeasy-api-schema-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Code Samples API
  slug: speakeasy-api-code-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Generation Events API
  slug: speakeasy-api-generation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Reports API
  slug: speakeasy-api-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy GitHub Automation API
  slug: speakeasy-api-github-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Suggest (OpenAPI AI) API
  slug: speakeasy-api-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Auth API
  slug: speakeasy-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Publishing Tokens API
  slug: speakeasy-api-publishing-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
- filename: speakeasy-api-openapi.yaml
  format: yaml
  label: Speakeasy Subscriptions API
  slug: speakeasy-api-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/openapi/speakeasy-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: speakeasy.com
  spf: true
  spf_policy: v=spf1 include:_spf.google.com -all
hosts:
- cert_expires: Sep 12 23:37:01 2026 GMT
  cert_issuer: Let's Encrypt
  host: www.speakeasy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 21:50:08 2026 GMT
  cert_issuer: Let's Encrypt
  host: speakeasy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:17:18 2026 GMT
  cert_issuer: Let's Encrypt
  host: api.prod.speakeasy.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speakeasy Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speakeasy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Speakeasy
provider_slug: speakeasy-api
slug: speakeasy-api-domain-security
source_filename: speakeasy-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.speakeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 12 23:37:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: speakeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep  9 21:50:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prod.speakeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt\n  cert_expires: Sep 26 13:17:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: speakeasy.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: 'v=spf1 include:_spf.google.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speakeasy-api/refs/heads/main/security/speakeasy-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Lifecycle
- SDK Generation
- Client Library
- API Design
- Developer Tools
- OpenAPI
- Code Generation
- Terraform
- MCP
- Developer Experience
---
