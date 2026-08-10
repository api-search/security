---
api_specs:
- filename: securitize-apac-api-openapi.yml
  format: yaml
  label: Securitize APAC API
  slug: securitize-apac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-apac-api-openapi.yml
- filename: securitize-domains-api-openapi.yml
  format: yaml
  label: Securitize Domains API
  slug: securitize-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-domains-api-openapi.yml
- filename: securitize-health-check-api-openapi.yml
  format: yaml
  label: Securitize Health Check API
  slug: securitize-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-health-check-api-openapi.yml
- filename: securitize-travel-rule-api-openapi.yml
  format: yaml
  label: Securitize Travel Rule API
  slug: securitize-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-travel-rule-api-openapi.yml
- filename: securitize-webhooks-api-openapi.yml
  format: yaml
  label: Securitize Webhooks API
  slug: securitize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: securitize.io
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: securitize.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 00:57:05 2026 GMT
  host: domain-api-docs.securitize.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: public-api.securitize.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Securitize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Securitize, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Securitize
provider_slug: securitize
slug: securitize-domain-security
source_filename: securitize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: securitize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: domain-api-docs.securitize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 00:57:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.securitize.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: securitize.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/security/securitize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- tokenization
- digital-securities
- real-world-assets
- capital-markets
- fund-administration
- transfer-agent
- kyc
- aml
- identity-verification
- blockchain
- broker-dealer
- private-credit
- mcp
- webhooks
---
