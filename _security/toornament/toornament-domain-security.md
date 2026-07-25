---
api_specs:
- filename: toornament-disciplines-api-openapi.yml
  format: yaml
  label: Toornament Disciplines API
  slug: toornament-disciplines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-disciplines-api-openapi.yml
- filename: toornament-matches-api-openapi.yml
  format: yaml
  label: Toornament Matches API
  slug: toornament-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-matches-api-openapi.yml
- filename: toornament-participants-api-openapi.yml
  format: yaml
  label: Toornament Participants API
  slug: toornament-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-participants-api-openapi.yml
- filename: toornament-rankings-api-openapi.yml
  format: yaml
  label: Toornament Rankings API
  slug: toornament-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-rankings-api-openapi.yml
- filename: toornament-registrations-api-openapi.yml
  format: yaml
  label: Toornament Registrations API
  slug: toornament-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-registrations-api-openapi.yml
- filename: toornament-stages-api-openapi.yml
  format: yaml
  label: Toornament Stages API
  slug: toornament-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-stages-api-openapi.yml
- filename: toornament-tournaments-api-openapi.yml
  format: yaml
  label: Toornament Tournaments API
  slug: toornament-tournaments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-tournaments-api-openapi.yml
- filename: toornament-webhooks-api-openapi.yml
  format: yaml
  label: Toornament Webhooks API
  slug: toornament-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/openapi/toornament-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: toornament.com
  spf: true
hosts:
- cert_expires: Sep  5 08:42:27 2026 GMT
  host: www.toornament.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:42:27 2026 GMT
  host: developer.toornament.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:42:27 2026 GMT
  host: api.toornament.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toornament Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toornament, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Toornament
provider_slug: toornament
slug: toornament-domain-security
source_filename: toornament-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toornament.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.toornament.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.toornament.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:42:27 2026 GMT\n  hsts: null\ndomains:\n- domain: toornament.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toornament/refs/heads/main/security/toornament-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Esports
- Gaming
- Tournaments
- Brackets
- Competition
---
