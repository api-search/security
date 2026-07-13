---
api_specs:
- filename: tint-openapi.yml
  format: yaml
  label: Tint Programs API
  slug: tint-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Quotes API
  slug: tint-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Policies API
  slug: tint-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Claims API
  slug: tint-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Decisions API
  slug: tint-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Questionnaires API
  slug: tint-questionnaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
- filename: tint-openapi.yml
  format: yaml
  label: Tint Webhooks API
  slug: tint-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/openapi/tint-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tint.ai
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.tint.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 22:12:33 2026 GMT
  host: docs.tint.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:20:07 2026 GMT
  host: api.tint.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tint
provider_slug: tint
slug: tint-domain-security
source_filename: tint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tint.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.tint.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:12:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tint.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:20:07 2026 GMT\n  hsts: null\ndomains:\n- domain: tint.ai\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tint/refs/heads/main/security/tint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Embedded Insurance
- InsurTech
- Insurance as a Service
- Protection
---
