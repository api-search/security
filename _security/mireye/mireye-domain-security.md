---
api_specs:
- filename: mireye-ask-api-openapi.yml
  format: yaml
  label: Mireye Ask API
  slug: mireye-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-ask-api-openapi.yml
- filename: mireye-ask-site-api-openapi.yml
  format: yaml
  label: Mireye Ask Site API
  slug: mireye-ask-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-ask-site-api-openapi.yml
- filename: mireye-auth-api-openapi.yml
  format: yaml
  label: Mireye Auth API
  slug: mireye-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-auth-api-openapi.yml
- filename: mireye-authorize-api-openapi.yml
  format: yaml
  label: Mireye Authorize API
  slug: mireye-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-authorize-api-openapi.yml
- filename: mireye-feature-requests-api-openapi.yml
  format: yaml
  label: Mireye Feature Requests API
  slug: mireye-feature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-feature-requests-api-openapi.yml
- filename: mireye-fetch-api-openapi.yml
  format: yaml
  label: Mireye Fetch API
  slug: mireye-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-fetch-api-openapi.yml
- filename: mireye-healthz-api-openapi.yml
  format: yaml
  label: Mireye Healthz API
  slug: mireye-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-healthz-api-openapi.yml
- filename: mireye-mcp-api-openapi.yml
  format: yaml
  label: Mireye Mcp API
  slug: mireye-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-mcp-api-openapi.yml
- filename: mireye-meta-api-openapi.yml
  format: yaml
  label: Mireye Meta API
  slug: mireye-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-meta-api-openapi.yml
- filename: mireye-oauth-api-openapi.yml
  format: yaml
  label: Mireye Oauth API
  slug: mireye-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-oauth-api-openapi.yml
- filename: mireye-readyz-api-openapi.yml
  format: yaml
  label: Mireye Readyz API
  slug: mireye-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-readyz-api-openapi.yml
- filename: mireye-register-api-openapi.yml
  format: yaml
  label: Mireye Register API
  slug: mireye-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-register-api-openapi.yml
- filename: mireye-revoke-api-openapi.yml
  format: yaml
  label: Mireye Revoke API
  slug: mireye-revoke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-revoke-api-openapi.yml
- filename: mireye-sites-api-openapi.yml
  format: yaml
  label: Mireye Sites API
  slug: mireye-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-sites-api-openapi.yml
- filename: mireye-token-api-openapi.yml
  format: yaml
  label: Mireye Token API
  slug: mireye-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-token-api-openapi.yml
- filename: mireye-users-api-openapi.yml
  format: yaml
  label: Mireye Users API
  slug: mireye-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-users-api-openapi.yml
- filename: mireye-well-known-api-openapi.yml
  format: yaml
  label: Mireye .well Known API
  slug: mireye-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mireye.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mireye.com
  spf: true
hosts:
- cert_expires: Aug 23 09:37:06 2026 GMT
  host: docs.mireye.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:35:34 2026 GMT
  host: api.mireye.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mireye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mireye, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Mireye
provider_slug: mireye
slug: mireye-domain-security
source_filename: mireye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mireye.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:37:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mireye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:35:34 2026 GMT\n  hsts: null\ndomains:\n- domain: mireye.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mireye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/security/mireye-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Geospatial
- Geographic Information System
- Location
- AI Agents
- Model Context Protocol
- Government Data
- Risk
- Insurance
- Data
---
