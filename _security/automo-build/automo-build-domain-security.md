---
api_specs:
- filename: automo-build-agent-api-openapi.yml
  format: yaml
  label: Automo Agent API
  slug: automo-build-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-agent-api-openapi.yml
- filename: automo-build-mcp-api-openapi.yml
  format: yaml
  label: Automo MCP API
  slug: automo-build-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-mcp-api-openapi.yml
- filename: automo-build-oauth-api-openapi.yml
  format: yaml
  label: Automo OAuth API
  slug: automo-build-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-oauth-api-openapi.yml
- filename: automo-build-openapi-json-api-openapi.yml
  format: yaml
  label: Automo Openapi.json API
  slug: automo-build-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-openapi-json-api-openapi.yml
- filename: automo-build-well-known-api-openapi.yml
  format: yaml
  label: Automo .well Known API
  slug: automo-build-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-well-known-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: automo.build
  spf: true
hosts:
- cert_expires: Jan  7 00:45:19 2027 GMT
  host: automo.build
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Automo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Automo
provider_slug: automo-build
slug: automo-build-domain-security
source_filename: automo-build-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: automo.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 00:45:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: automo.build\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/automo-build/security/automo-build-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Platform
- Low-Code
- Automation
- Software Development
---
