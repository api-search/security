---
api_specs:
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Reports API
  slug: goodhire-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Requestors API
  slug: goodhire-requestors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Packages API
  slug: goodhire-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Webhooks API
  slug: goodhire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
- filename: goodhire-openapi.yml
  format: yaml
  label: GoodHire Partner API
  slug: goodhire-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/openapi/goodhire-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodhire.com
  spf: true
hosts:
- cert_expires: Aug 12 11:33:51 2026 GMT
  host: www.goodhire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: api.goodhire.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: help.goodhire.com
  https: false
kind: domain-security
layout: security
method: probed
name: Goodhire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoodHire, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoodHire
provider_slug: goodhire
slug: goodhire-domain-security
source_filename: goodhire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodhire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 11:33:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.goodhire.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: help.goodhire.com\n  https: false\ndomains:\n- domain: goodhire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodhire/refs/heads/main/security/goodhire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Background Checks
- Employment Screening
- Identity Verification
- HR
- Compliance
- FCRA
- Checkr
---
