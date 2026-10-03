---
api_specs:
- filename: apono-api-reference-api-openapi.yml
  format: yaml
  label: Apono Api Reference API
  slug: apono-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apono/refs/heads/main/openapi/apono-api-reference-api-openapi.yml
- filename: apono-apono-api-api-openapi.yml
  format: yaml
  label: Apono Apono API
  slug: apono-apono-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apono/refs/heads/main/openapi/apono-apono-api-api-openapi.yml
- filename: apono-docs-api-openapi.yml
  format: yaml
  label: Apono Docs API
  slug: apono-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apono/refs/heads/main/openapi/apono-docs-api-openapi.yml
- filename: apono-user-api-openapi.yml
  format: yaml
  label: Apono User API
  slug: apono-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apono/refs/heads/main/openapi/apono-user-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: apono.io
  spf: true
hosts:
- cert_expires: Nov 13 09:58:25 2026 GMT
  host: www.apono.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 20:13:25 2026 GMT
  host: docs.apono.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Apono Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apono, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Apono
provider_slug: apono
slug: apono-domain-security
source_filename: apono-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apono.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 09:58:25 2026 GMT\n  hsts: false\n- host: docs.apono.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 20:13:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apono.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apono/refs/heads/main/security/apono-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Privileged Access Management
- Cloud Security
- Zero Standing Privilege
- AI Agents
- Identity Governance
---
