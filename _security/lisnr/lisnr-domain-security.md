---
api_specs:
- filename: lisnr-accounts-api-openapi.yml
  format: yaml
  label: LISNR Accounts API
  slug: lisnr-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-accounts-api-openapi.yml
- filename: lisnr-api-tokens-api-openapi.yml
  format: yaml
  label: LISNR API Tokens API
  slug: lisnr-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-api-tokens-api-openapi.yml
- filename: lisnr-applications-api-openapi.yml
  format: yaml
  label: LISNR Applications API
  slug: lisnr-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-applications-api-openapi.yml
- filename: lisnr-authentication-api-openapi.yml
  format: yaml
  label: LISNR Authentication API
  slug: lisnr-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-authentication-api-openapi.yml
- filename: lisnr-billing-api-openapi.yml
  format: yaml
  label: LISNR Billing API
  slug: lisnr-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-billing-api-openapi.yml
- filename: lisnr-notifications-api-openapi.yml
  format: yaml
  label: LISNR Notifications API
  slug: lisnr-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-notifications-api-openapi.yml
- filename: lisnr-sdk-releases-api-openapi.yml
  format: yaml
  label: LISNR SDK Releases API
  slug: lisnr-sdk-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-sdk-releases-api-openapi.yml
- filename: lisnr-sdk-tokens-api-openapi.yml
  format: yaml
  label: LISNR SDK Tokens API
  slug: lisnr-sdk-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-sdk-tokens-api-openapi.yml
- filename: lisnr-tones-service-api-reference-api-openapi.yml
  format: yaml
  label: LISNR Tones Service API Reference API
  slug: lisnr-tones-service-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-tones-service-api-reference-api-openapi.yml
- filename: lisnr-users-api-openapi.yml
  format: yaml
  label: LISNR Users API
  slug: lisnr-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/openapi/lisnr-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lisnr.com
  spf: true
hosts:
- cert_expires: Sep 11 02:26:27 2026 GMT
  host: lisnr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: portal.lisnr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: tones.lisnr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lisnr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LISNR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LISNR
provider_slug: lisnr
slug: lisnr-domain-security
source_filename: lisnr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lisnr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 02:26:27 2026 GMT\n  hsts: false\n- host: portal.lisnr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n- host: tones.lisnr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lisnr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lisnr/refs/heads/main/security/lisnr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ultrasonic
- Data Over Audio
- Proximity
- Contactless Payments
- Device Pairing
- Identification
- Audio
- Internet of Things
- SDK
---
