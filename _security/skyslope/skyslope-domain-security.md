---
api_specs:
- filename: skyslope-agents-listings-api-openapi.yml
  format: yaml
  label: SkySlope Agents, Listings API
  slug: skyslope-agents-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-agents-listings-api-openapi.yml
- filename: skyslope-auth-api-openapi.yml
  format: yaml
  label: SkySlope Auth API
  slug: skyslope-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-auth-api-openapi.yml
- filename: skyslope-buyer-agreements-api-openapi.yml
  format: yaml
  label: SkySlope Buyer Agreements API
  slug: skyslope-buyer-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-buyer-agreements-api-openapi.yml
- filename: skyslope-contacts-api-openapi.yml
  format: yaml
  label: SkySlope Contacts API
  slug: skyslope-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-contacts-api-openapi.yml
- filename: skyslope-documents-api-openapi.yml
  format: yaml
  label: SkySlope Documents API
  slug: skyslope-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-documents-api-openapi.yml
- filename: skyslope-envelopes-api-openapi.yml
  format: yaml
  label: SkySlope Envelopes API
  slug: skyslope-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-envelopes-api-openapi.yml
- filename: skyslope-files-api-openapi.yml
  format: yaml
  label: SkySlope Files API
  slug: skyslope-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-files-api-openapi.yml
- filename: skyslope-forms-api-openapi.yml
  format: yaml
  label: SkySlope Forms API
  slug: skyslope-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-forms-api-openapi.yml
- filename: skyslope-libraries-api-openapi.yml
  format: yaml
  label: SkySlope Libraries API
  slug: skyslope-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-libraries-api-openapi.yml
- filename: skyslope-offers-api-openapi.yml
  format: yaml
  label: SkySlope Offers API
  slug: skyslope-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-offers-api-openapi.yml
- filename: skyslope-report-api-openapi.yml
  format: yaml
  label: SkySlope Report API
  slug: skyslope-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-report-api-openapi.yml
- filename: skyslope-templates-api-openapi.yml
  format: yaml
  label: SkySlope Templates API
  slug: skyslope-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-templates-api-openapi.yml
- filename: skyslope-users-api-openapi.yml
  format: yaml
  label: SkySlope Users API
  slug: skyslope-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-users-api-openapi.yml
- filename: skyslope-webhooks-api-openapi.yml
  format: yaml
  label: SkySlope Webhooks API
  slug: skyslope-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/openapi/skyslope-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: skyslope.com
  spf: true
hosts:
- cert_expires: Oct  2 02:17:48 2026 GMT
  host: skyslope.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:17:48 2026 GMT
  host: forms.skyslope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:17:48 2026 GMT
  host: offers.skyslope.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skyslope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkySlope, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SkySlope
provider_slug: skyslope
slug: skyslope-domain-security
source_filename: skyslope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skyslope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:17:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: forms.skyslope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:17:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: offers.skyslope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:17:48 2026 GMT\n  hsts: false\ndomains:\n- domain: skyslope.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyslope/refs/heads/main/security/skyslope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Transaction Management
- Digital Forms
- E-Signature
- Compliance
- PropTech
- Documents
---
