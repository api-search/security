---
api_specs:
- filename: urjanet-openapi.yml
  format: yaml
  label: Urjanet Credentials & Connections API
  slug: urjanet-credentials-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-openapi.yml
- filename: urjanet-openapi.yml
  format: yaml
  label: Urjanet Statements & Bills API
  slug: urjanet-statements-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-openapi.yml
- filename: urjanet-openapi.yml
  format: yaml
  label: Urjanet Meters API
  slug: urjanet-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-openapi.yml
- filename: urjanet-openapi.yml
  format: yaml
  label: Urjanet Usage Data API
  slug: urjanet-usage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-openapi.yml
- filename: urjanet-openapi.yml
  format: yaml
  label: Urjanet Webhooks API
  slug: urjanet-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/openapi/urjanet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urjanet.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcadia.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: urjanet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:20:02 2026 GMT
  host: docs.arcadia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: api.urjanet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urjanet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urjanet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Urjanet
provider_slug: urjanet
slug: urjanet-domain-security
source_filename: urjanet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urjanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.urjanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: urjanet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: arcadia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urjanet/refs/heads/main/security/urjanet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Utility Data
- Energy
- Utility Bills
- Aggregation
- Meters
- Sustainability
---
