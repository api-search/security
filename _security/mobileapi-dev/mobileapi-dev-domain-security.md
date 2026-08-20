---
api_specs:
- filename: mobileapi-dev-api-api-openapi.yml
  format: yaml
  label: MobileAPI.dev api API
  slug: mobileapi-dev-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-api-api-openapi.yml
- filename: mobileapi-dev-api-token-auth-api-openapi.yml
  format: yaml
  label: MobileAPI.dev api-token-auth API
  slug: mobileapi-dev-api-token-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-api-token-auth-api-openapi.yml
- filename: mobileapi-dev-demo-x7k9m2p4-api-openapi.yml
  format: yaml
  label: MobileAPI.dev demo-x7k9m2p4 API
  slug: mobileapi-dev-demo-x7k9m2p4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-demo-x7k9m2p4-api-openapi.yml
- filename: mobileapi-dev-devices-api-openapi.yml
  format: yaml
  label: MobileAPI.dev devices API
  slug: mobileapi-dev-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-devices-api-openapi.yml
- filename: mobileapi-dev-images-api-openapi.yml
  format: yaml
  label: MobileAPI.dev images API
  slug: mobileapi-dev-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-images-api-openapi.yml
- filename: mobileapi-dev-manufacturers-api-openapi.yml
  format: yaml
  label: MobileAPI.dev manufacturers API
  slug: mobileapi-dev-manufacturers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-manufacturers-api-openapi.yml
- filename: mobileapi-dev-me-api-openapi.yml
  format: yaml
  label: MobileAPI.dev me API
  slug: mobileapi-dev-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-me-api-openapi.yml
- filename: mobileapi-dev-payment-successful-api-openapi.yml
  format: yaml
  label: MobileAPI.dev payment_successful API
  slug: mobileapi-dev-payment-successful-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-payment-successful-api-openapi.yml
- filename: mobileapi-dev-status-api-openapi.yml
  format: yaml
  label: MobileAPI.dev status API
  slug: mobileapi-dev-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/openapi/mobileapi-dev-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mobileapi.dev
  spf: true
hosts:
- cert_expires: Sep  5 08:12:11 2026 GMT
  host: mobileapi.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:12:11 2026 GMT
  host: api.mobileapi.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mobileapi Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MobileAPI.dev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MobileAPI.dev
provider_slug: mobileapi-dev
slug: mobileapi-dev-domain-security
source_filename: mobileapi-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobileapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:12:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mobileapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:12:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mobileapi.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobileapi-dev/refs/heads/main/security/mobileapi-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data API
- Developer Tools
- Device Specifications
- Mobile Data
- Phone Specs
- REST API
- Software-as-a-Service
---
