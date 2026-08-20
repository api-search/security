---
api_specs:
- filename: speakeasy-artifacts-api-openapi.yml
  format: yaml
  label: Speakeasy Artifacts API
  slug: speakeasy-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-artifacts-api-openapi.yml
- filename: speakeasy-auth-api-openapi.yml
  format: yaml
  label: Speakeasy Auth API
  slug: speakeasy-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-auth-api-openapi.yml
- filename: speakeasy-codesamples-api-openapi.yml
  format: yaml
  label: Speakeasy CodeSamples API
  slug: speakeasy-codesamples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-codesamples-api-openapi.yml
- filename: speakeasy-events-api-openapi.yml
  format: yaml
  label: Speakeasy Events API
  slug: speakeasy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-events-api-openapi.yml
- filename: speakeasy-github-api-openapi.yml
  format: yaml
  label: Speakeasy Github API
  slug: speakeasy-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-github-api-openapi.yml
- filename: speakeasy-organizations-api-openapi.yml
  format: yaml
  label: Speakeasy Organizations API
  slug: speakeasy-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-organizations-api-openapi.yml
- filename: speakeasy-publishingtokens-api-openapi.yml
  format: yaml
  label: Speakeasy PublishingTokens API
  slug: speakeasy-publishingtokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-publishingtokens-api-openapi.yml
- filename: speakeasy-reports-api-openapi.yml
  format: yaml
  label: Speakeasy Reports API
  slug: speakeasy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-reports-api-openapi.yml
- filename: speakeasy-schemastore-api-openapi.yml
  format: yaml
  label: Speakeasy SchemaStore API
  slug: speakeasy-schemastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-schemastore-api-openapi.yml
- filename: speakeasy-shorturls-api-openapi.yml
  format: yaml
  label: Speakeasy ShortURLs API
  slug: speakeasy-shorturls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-shorturls-api-openapi.yml
- filename: speakeasy-subscriptions-api-openapi.yml
  format: yaml
  label: Speakeasy Subscriptions API
  slug: speakeasy-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-subscriptions-api-openapi.yml
- filename: speakeasy-suggest-api-openapi.yml
  format: yaml
  label: Speakeasy Suggest API
  slug: speakeasy-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-suggest-api-openapi.yml
- filename: speakeasy-workspaces-api-openapi.yml
  format: yaml
  label: Speakeasy Workspaces API
  slug: speakeasy-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/openapi/speakeasy-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: speakeasy.com
  spf: true
hosts:
- cert_expires: Sep 12 23:37:01 2026 GMT
  host: www.speakeasy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:17:18 2026 GMT
  host: api.prod.speakeasy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speakeasy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Speakeasy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Speakeasy
provider_slug: speakeasy
slug: speakeasy-domain-security
source_filename: speakeasy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.speakeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:37:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prod.speakeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:17:18 2026 GMT\n  hsts: null\ndomains:\n- domain: speakeasy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speakeasy/refs/heads/main/security/speakeasy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Documentation
- MCP
- Platform
- SDK
- Terraform
- Testing
---
