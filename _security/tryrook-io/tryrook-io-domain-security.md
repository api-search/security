---
api_specs:
- filename: tryrook-io-client-uuid-api-openapi.yml
  format: yaml
  label: ROOK Client Uuid API
  slug: tryrook-io-client-uuid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/openapi/tryrook-io-client-uuid-api-openapi.yml
- filename: tryrook-io-extraction-app-api-openapi.yml
  format: yaml
  label: ROOK Extraction App API
  slug: tryrook-io-extraction-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/openapi/tryrook-io-extraction-app-api-openapi.yml
- filename: tryrook-io-user-id-api-openapi.yml
  format: yaml
  label: ROOK User Id API
  slug: tryrook-io-user-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/openapi/tryrook-io-user-id-api-openapi.yml
- filename: tryrook-io-user-profile-api-openapi.yml
  format: yaml
  label: ROOK User Profile API
  slug: tryrook-io-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/openapi/tryrook-io-user-profile-api-openapi.yml
- filename: tryrook-io-webhooks-api-openapi.yml
  format: yaml
  label: ROOK Webhooks API
  slug: tryrook-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/openapi/tryrook-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tryrook.io
  spf: true
hosts:
- cert_expires: Apr 21 20:15:19 2027 GMT
  host: www.tryrook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tryrook Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ROOK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ROOK
provider_slug: tryrook-io
slug: tryrook-io-domain-security
source_filename: tryrook-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryrook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 21 20:15:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tryrook.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tryrook-io/refs/heads/main/security/tryrook-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health
- Data Integration
- Wearables
- Healthcare
---
