---
api_specs:
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Programs API
  slug: boost-insurance-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Quotes API
  slug: boost-insurance-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Policies API
  slug: boost-insurance-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Claims API
  slug: boost-insurance-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Endorsements API
  slug: boost-insurance-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Webhooks API
  slug: boost-insurance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boostinsurance.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: insurtech.dev
  spf: false
hosts:
- cert_expires: Sep 28 14:31:31 2026 GMT
  host: www.boostinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 05:38:08 2026 GMT
  host: learn.boostinsurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.insurtech.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Boost Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boost Insurance, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boost Insurance
provider_slug: boost-insurance
slug: boost-insurance-domain-security
source_filename: boost-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boostinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.boostinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.insurtech.dev\n  https: false\ndomains:\n- domain: boostinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: insurtech.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/security/boost-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Embedded Insurance
- Insurance-as-a-Service
- Policy Administration
- Claims
---
