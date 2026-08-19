---
api_specs:
- filename: dotfile-cases-openapi.yml
  format: yaml
  label: Dotfile API
  slug: dotfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotfile/refs/heads/main/openapi/dotfile-cases-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dotfile.com
  spf: true
hosts:
- cert_expires: Oct 31 07:05:34 2026 GMT
  host: www.dotfile.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 15:06:36 2026 GMT
  host: docs.dotfile.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.dotfile.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dotfile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dotfile, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dotfile
provider_slug: dotfile
slug: dotfile-domain-security
source_filename: dotfile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dotfile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 07:05:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.dotfile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 15:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dotfile.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dotfile.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotfile/refs/heads/main/security/dotfile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- kyb
- kyc
- aml
- business-verification
- identity-verification
- compliance
- regtech
- onboarding
- sanctions-screening
- document-verification
- fraud-detection
- company-data
- beneficial-ownership
- case-management
- electronic-signature
- webhooks
---
