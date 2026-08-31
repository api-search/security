---
api_specs:
- filename: abloatai-branches-api-openapi.yml
  format: yaml
  label: Ablo Branches API
  slug: ablo-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-branches-api-openapi.yml
- filename: abloatai-claims-api-openapi.yml
  format: yaml
  label: Ablo Claims API
  slug: ablo-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-claims-api-openapi.yml
- filename: abloatai-commits-api-openapi.yml
  format: yaml
  label: Ablo Commits API
  slug: ablo-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-commits-api-openapi.yml
- filename: abloatai-credentials-api-openapi.yml
  format: yaml
  label: Ablo Credentials API
  slug: ablo-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-credentials-api-openapi.yml
- filename: abloatai-logs-api-openapi.yml
  format: yaml
  label: Ablo Logs API
  slug: ablo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-logs-api-openapi.yml
- filename: abloatai-models-api-openapi.yml
  format: yaml
  label: Ablo Models API
  slug: ablo-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-models-api-openapi.yml
- filename: abloatai-schema-api-openapi.yml
  format: yaml
  label: Ablo Schema API
  slug: ablo-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/openapi/abloatai-schema-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abloatai.com
  spf: false
hosts:
- cert_expires: Oct 24 08:31:54 2026 GMT
  host: docs.abloatai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.abloatai.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'The automated probe recorded hsts: null because the host root returns a JSON 404; a live GET of https://api.abloatai.com/api/v1/schema returns strict-transport-security: max-age=31536000; includeSubDomains. Corrected from direct observation.'
  https: true
  security_headers:
    content-security-policy: default-src 'none'; frame-ancestors 'none'
    permissions-policy: geolocation=(), microphone=(), camera=()
    referrer-policy: strict-origin-when-cross-origin
    x-content-type-options: nosniff
    x-frame-options: DENY
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abloatai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ablo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ablo
provider_slug: abloatai
slug: abloatai-domain-security
source_filename: abloatai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.abloatai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 08:31:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.abloatai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: 'The automated probe recorded hsts: null because the host root returns a JSON 404; a live GET of https://api.abloatai.com/api/v1/schema\n    returns strict-transport-security: max-age=31536000; includeSubDomains. Corrected from direct observation.'\n  security_headers:\n    content-security-policy: default-src 'none'; frame-ancestors 'none'\n    x-content-type-options: nosniff\n    x-frame-options: DENY\n    referrer-policy: strict-origin-when-cross-origin\n    permissions-policy: geolocation=(), microphone=(), camera=()\ndomains:\n\
  - domain: abloatai.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\nnote: 'Probed with 0-working/probe-domain-security.py, then the api.abloatai.com HSTS field was corrected from a\n  direct observation of a live authenticated-path response. Notable gaps: no DNSSEC and no SPF record on abloatai.com,\n  and DMARC is published at p=none (monitor only), so the domain is not yet protected against spoofing. CAA is present\n  and restrictive.'\ngaps:\n- no DNSSEC\n- no SPF record\n- DMARC policy is p=none (monitoring only, not enforcing)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abloatai/refs/heads/main/security/abloatai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- agent-infrastructure
- multi-agent-coordination
- concurrency-control
- state-management
- Database
- postgres
- real-time-sync
- MCP
- Developer Tools
- backend-infrastructure
---
