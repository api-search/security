---
api_specs:
- filename: 0codekit-ai-api-openapi.yml
  format: yaml
  label: relyon AI API
  slug: 0codekit-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-ai-api-openapi.yml
- filename: 0codekit-docs-api-openapi.yml
  format: yaml
  label: relyon Docs API
  slug: 0codekit-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-docs-api-openapi.yml
- filename: 0codekit-image-api-openapi.yml
  format: yaml
  label: relyon Image API
  slug: 0codekit-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-image-api-openapi.yml
- filename: 0codekit-mcp-api-openapi.yml
  format: yaml
  label: relyon MCP API
  slug: 0codekit-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-mcp-api-openapi.yml
- filename: 0codekit-pdf-api-openapi.yml
  format: yaml
  label: relyon PDF API
  slug: 0codekit-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/openapi/0codekit-pdf-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/3800395326;validationmethods=dns-01"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 0codekit.com
  spf: false
hosts:
- cert_expires: Nov 26 08:12:44 2026 GMT
  host: 0codekit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 0Codekit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for relyon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: relyon
provider_slug: 0codekit
slug: 0codekit-domain-security
source_filename: 0codekit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 0codekit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 08:12:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 0codekit.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/3800395326;validationmethods=dns-01\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0codekit/refs/heads/main/security/0codekit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Low-Code
- No-Code
- PDF Tools
- AI Integration
---
