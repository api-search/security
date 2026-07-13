---
api_specs:
- filename: certn-openapi.yml
  format: yaml
  label: Certn Applications API
  slug: certn-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Checks API
  slug: certn-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Reports API
  slug: certn-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Packages API
  slug: certn-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Webhooks API
  slug: certn-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
- filename: certn-openapi.yml
  format: yaml
  label: Certn Teams and Users API
  slug: certn-teams-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/openapi/certn-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: certn.co
  spf: true
hosts:
- cert_expires: Aug 26 01:03:04 2026 GMT
  host: certn.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 13:06:01 2026 GMT
  host: docs.certn.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 01:03:04 2026 GMT
  host: api.certn.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Certn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Certn
provider_slug: certn
slug: certn-domain-security
source_filename: certn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.certn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.certn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: certn.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certn/refs/heads/main/security/certn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Background Checks
- Identity Verification
- Criminal Record Check
- Screening
- HR Tech
- Compliance
- Trust and Safety
---
