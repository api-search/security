---
api_specs:
- filename: telkomsel-consent-management-api-openapi.yml
  format: yaml
  label: Telkomsel Consent Management API
  slug: telkomsel-consent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-consent-management-api-openapi.yml
- filename: telkomsel-identity-verification-api-openapi.yml
  format: yaml
  label: Telkomsel Identity Verification API
  slug: telkomsel-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-identity-verification-api-openapi.yml
- filename: telkomsel-location-api-openapi.yml
  format: yaml
  label: Telkomsel Location API
  slug: telkomsel-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-location-api-openapi.yml
- filename: telkomsel-scoring-and-insights-api-openapi.yml
  format: yaml
  label: Telkomsel Scoring and Insights API
  slug: telkomsel-scoring-and-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-scoring-and-insights-api-openapi.yml
- filename: telkomsel-sim-swap-api-openapi.yml
  format: yaml
  label: Telkomsel SIM Swap API
  slug: telkomsel-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-sim-swap-api-openapi.yml
- filename: telkomsel-sms-api-openapi.yml
  format: yaml
  label: Telkomsel SMS API
  slug: telkomsel-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-sms-api-openapi.yml
- filename: telkomsel-subscriber-check-api-openapi.yml
  format: yaml
  label: Telkomsel Subscriber Check API
  slug: telkomsel-subscriber-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-subscriber-check-api-openapi.yml
- filename: telkomsel-ussd-api-openapi.yml
  format: yaml
  label: Telkomsel USSD API
  slug: telkomsel-ussd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/openapi/telkomsel-ussd-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telkomsel.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: www.telkomsel.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: digihub.telkomsel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: api.digitalcore.telkomsel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telkomsel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telkomsel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Telkomsel
provider_slug: telkomsel
slug: telkomsel-domain-security
source_filename: telkomsel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telkomsel.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: digihub.telkomsel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.digitalcore.telkomsel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: telkomsel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telkomsel/refs/heads/main/security/telkomsel-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Telecommunications
- Indonesia
- SMS
- Mobile Network
- CPaaS
- Network APIs
- Identity Verification
---
