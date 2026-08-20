---
api_specs:
- filename: pact-index-api-openapi.yml
  format: yaml
  label: Pact Index API
  slug: pact-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-index-api-openapi.yml
- filename: pact-pacticipants-api-openapi.yml
  format: yaml
  label: Pact Pacticipants API
  slug: pact-pacticipants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-pacticipants-api-openapi.yml
- filename: pact-pacts-api-openapi.yml
  format: yaml
  label: Pact Pacts API
  slug: pact-pacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-pacts-api-openapi.yml
- filename: pact-verifications-api-openapi.yml
  format: yaml
  label: Pact Verifications API
  slug: pact-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-verifications-api-openapi.yml
- filename: pact-webhooks-api-openapi.yml
  format: yaml
  label: Pact Webhooks API
  slug: pact-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/openapi/pact-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pact.io
  spf: false
hosts:
- cert_expires: Sep  2 02:43:56 2026 GMT
  host: pact.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:33:41 2026 GMT
  host: docs.pact.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pact, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Pact
provider_slug: pact
slug: pact-domain-security
source_filename: pact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pact.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:43:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pact.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pact.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pact/refs/heads/main/security/pact-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Contract Testing
- Open-Source
- Testing
---
