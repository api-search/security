---
api_specs:
- filename: codefmt-dev-ask-api-openapi.yml
  format: yaml
  label: codefmt Ask API
  slug: codefmt-dev-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codefmt-dev/openapi/codefmt-dev-ask-api-openapi.yml
- filename: codefmt-dev-format-api-openapi.yml
  format: yaml
  label: codefmt Format API
  slug: codefmt-dev-format-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codefmt-dev/openapi/codefmt-dev-format-api-openapi.yml
- filename: codefmt-dev-health-api-openapi.yml
  format: yaml
  label: codefmt Health API
  slug: codefmt-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codefmt-dev/openapi/codefmt-dev-health-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:tlsrpt@codefmt.dev"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: codefmt.dev
  spf: true
hosts:
- cert_expires: Dec 29 21:25:13 2026 GMT
  host: codefmt.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: codefmt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for codefmt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: codefmt
provider_slug: codefmt-dev
slug: codefmt-dev-domain-security
source_filename: codefmt-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codefmt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 21:25:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codefmt.dev\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:tlsrpt@codefmt.dev\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/codefmt-dev/security/codefmt-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Code Formatting
- Linting
- HubL
- HubSpot
- Zapier
- n8n
- Automation
- Developer Tools
- MCP
---
