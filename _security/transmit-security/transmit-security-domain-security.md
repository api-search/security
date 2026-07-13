---
api_specs:
- filename: api_ref_intro
  format: yaml
  label: Mosaic Identity Management, Authentication & Journeys API
  slug: mosaic-identity-management-authentication-journeys-api
  spec_type: OpenAPI
  url: https://developer.transmitsecurity.com/openapi/api_ref_intro
- filename: api_ref_intro
  format: yaml
  label: Mosaic Fraud Prevention API
  slug: mosaic-fraud-prevention-api
  spec_type: OpenAPI
  url: https://developer.transmitsecurity.com/openapi/api_ref_intro
- filename: api_ref_intro
  format: yaml
  label: Mosaic Identity Verification API
  slug: mosaic-identity-verification-api
  spec_type: OpenAPI
  url: https://developer.transmitsecurity.com/openapi/api_ref_intro
- filename: transmit-security-platform-administration-openapi.yml
  format: yaml
  label: Mosaic Platform Administration API
  slug: mosaic-platform-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transmit-security/refs/heads/main/openapi/transmit-security-platform-administration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transmitsecurity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transmitsecurity.io
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: transmitsecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 18:47:07 2026 GMT
  host: developer.transmitsecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 13:16:22 2026 GMT
  host: api.transmitsecurity.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transmit Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transmit Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transmit Security
provider_slug: transmit-security
slug: transmit-security-domain-security
source_filename: transmit-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transmitsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.transmitsecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:47:07 2026 GMT\n  hsts: false\n- host: api.transmitsecurity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:16:22 2026 GMT\n  hsts: null\ndomains:\n- domain: transmitsecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: transmitsecurity.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transmit-security/refs/heads/main/security/transmit-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CIAM
- Identity
- Authentication
- Passkeys
- WebAuthn
- Fraud Detection
- Risk Management
- Identity Verification
- Orchestration
- OAuth2
- Security
- SSO
---
