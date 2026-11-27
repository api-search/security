---
api_specs:
- filename: corroborateme-com-agents-api-openapi.yml
  format: yaml
  label: CorroborateMe Agents API
  slug: corroborateme-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-agents-api-openapi.yml
- filename: corroborateme-com-billing-api-openapi.yml
  format: yaml
  label: CorroborateMe Billing API
  slug: corroborateme-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-billing-api-openapi.yml
- filename: corroborateme-com-companies-api-openapi.yml
  format: yaml
  label: CorroborateMe Companies API
  slug: corroborateme-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-companies-api-openapi.yml
- filename: corroborateme-com-console-auth-api-openapi.yml
  format: yaml
  label: CorroborateMe Console auth API
  slug: corroborateme-com-console-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-console-auth-api-openapi.yml
- filename: corroborateme-com-discovery-api-openapi.yml
  format: yaml
  label: CorroborateMe Discovery API
  slug: corroborateme-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-discovery-api-openapi.yml
- filename: corroborateme-com-integrations-api-openapi.yml
  format: yaml
  label: CorroborateMe Integrations API
  slug: corroborateme-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-integrations-api-openapi.yml
- filename: corroborateme-com-login-link-idp-api-openapi.yml
  format: yaml
  label: CorroborateMe Login-link IdP API
  slug: corroborateme-com-login-link-idp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-login-link-idp-api-openapi.yml
- filename: corroborateme-com-login-links-api-openapi.yml
  format: yaml
  label: CorroborateMe Login links API
  slug: corroborateme-com-login-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-login-links-api-openapi.yml
- filename: corroborateme-com-mcp-api-openapi.yml
  format: yaml
  label: CorroborateMe MCP API
  slug: corroborateme-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-mcp-api-openapi.yml
- filename: corroborateme-com-oidc-api-openapi.yml
  format: yaml
  label: CorroborateMe OIDC API
  slug: corroborateme-com-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corroborateme-com/openapi/corroborateme-com-oidc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corroborateme.com
  spf: true
hosts:
- cert_expires: Dec 13 21:46:22 2026 GMT
  host: corroborateme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CorroborateMe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CorroborateMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CorroborateMe
provider_slug: corroborateme-com
slug: corroborateme-com-domain-security
source_filename: corroborateme-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corroborateme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 21:46:22 2026 GMT\n  hsts: false\ndomains:\n- domain: corroborateme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/corroborateme-com/security/corroborateme-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Authentication
- Identity
- Sign In
- Passkeys
- OpenID Connect
- SSO
- AI Agents
- MCP
---
