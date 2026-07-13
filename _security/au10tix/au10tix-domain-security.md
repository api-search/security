---
api_specs:
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Identity Verification API
  slug: au10tix-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Document Authentication API
  slug: au10tix-document-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Face Comparison & Liveness API
  slug: au10tix-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Results API
  slug: au10tix-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Webhooks API
  slug: au10tix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: au10tix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: au10tixservices.com
  spf: false
hosts:
- cert_expires: Oct  1 13:12:29 2026 GMT
  host: www.au10tix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 10:24:00 2026 GMT
  host: eus-api.au10tixservices.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: euxbos.cloudapp.net
  https: false
kind: domain-security
layout: security
method: probed
name: Au10Tix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AU10TIX, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AU10TIX
provider_slug: au10tix
slug: au10tix-domain-security
source_filename: au10tix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.au10tix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 13:12:29 2026 GMT\n  hsts: false\n- host: eus-api.au10tixservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 10:24:00 2026 GMT\n  hsts: null\n- host: euxbos.cloudapp.net\n  https: false\ndomains:\n- domain: au10tix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: au10tixservices.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/security/au10tix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity Verification
- Document Authentication
- KYC
- Biometrics
- Fraud Detection
---
