---
api_specs:
- filename: vynedental-eligibility-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility and Benefits API (Onederful)
  slug: eligibility-and-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-api-openapi.yml
- filename: vynedental-async-api-openapi.yml
  format: yaml
  label: Vyne Dental Async API
  slug: vynedental-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-async-api-openapi.yml
- filename: vynedental-edi-api-openapi.yml
  format: yaml
  label: Vyne Dental EDI API
  slug: vynedental-edi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-edi-api-openapi.yml
- filename: vynedental-eligibility-response-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility Response API
  slug: vynedental-eligibility-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-response-api-openapi.yml
- filename: vynedental-eligibility-status-api-openapi.yml
  format: yaml
  label: Vyne Dental Eligibility Status API
  slug: vynedental-eligibility-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-eligibility-status-api-openapi.yml
- filename: vynedental-enhanced-eligibility-api-openapi.yml
  format: yaml
  label: Vyne Dental Enhanced Eligibility API
  slug: vynedental-enhanced-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-enhanced-eligibility-api-openapi.yml
- filename: vynedental-oauth2-api-openapi.yml
  format: yaml
  label: Vyne Dental Oauth2 API
  slug: vynedental-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-oauth2-api-openapi.yml
- filename: vynedental-well-known-api-openapi.yml
  format: yaml
  label: Vyne Dental .well Known API
  slug: vynedental-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/openapi/vynedental-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vynedental.com
  spf: true
hosts:
- cert_expires: Dec 20 08:04:51 2026 GMT
  host: vynedental.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vynedental Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vyne Dental, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vyne Dental
provider_slug: vynedental
slug: vynedental-domain-security
source_filename: vynedental-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vynedental.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 08:04:51 2026 GMT\n  hsts: false\ndomains:\n- domain: vynedental.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vynedental/refs/heads/main/security/vynedental-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Dental
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- Payments
---
