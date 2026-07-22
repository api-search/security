---
api_specs:
- filename: monaco-openapi-original.json
  format: json
  label: Monaco Public API
  slug: monaco-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/openapi/monaco-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@monaco.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monaco.com
  spf: true
hosts:
- cert_expires: Sep 11 09:08:35 2026 GMT
  host: www.monaco.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 03:33:31 2026 GMT
  host: docs.monaco.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.monaco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monaco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monaco, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Monaco
provider_slug: monaco
slug: monaco-domain-security
source_filename: monaco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monaco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:08:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.monaco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.monaco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: monaco.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@monaco.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monaco/refs/heads/main/security/monaco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- CRM
- Sales
- Revenue Operations
- Artificial Intelligence
- Contacts
- Accounts
- Opportunities
- Pipeline
- Go To Market
- MCP
---
