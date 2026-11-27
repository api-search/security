---
api_specs:
- filename: ffraud-com-account-api-openapi.yml
  format: yaml
  label: FFraud Account API
  slug: ffraud-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-account-api-openapi.yml
- filename: ffraud-com-community-api-openapi.yml
  format: yaml
  label: FFraud Community API
  slug: ffraud-com-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-community-api-openapi.yml
- filename: ffraud-com-compatibility-api-openapi.yml
  format: yaml
  label: FFraud Compatibility API
  slug: ffraud-com-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-compatibility-api-openapi.yml
- filename: ffraud-com-device-api-openapi.yml
  format: yaml
  label: FFraud Device API
  slug: ffraud-com-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-device-api-openapi.yml
- filename: ffraud-com-domain-api-openapi.yml
  format: yaml
  label: FFraud Domain API
  slug: ffraud-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-domain-api-openapi.yml
- filename: ffraud-com-email-api-openapi.yml
  format: yaml
  label: FFraud Email API
  slug: ffraud-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-email-api-openapi.yml
- filename: ffraud-com-ip-api-openapi.yml
  format: yaml
  label: FFraud IP API
  slug: ffraud-com-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-ip-api-openapi.yml
- filename: ffraud-com-system-api-openapi.yml
  format: yaml
  label: FFraud System API
  slug: ffraud-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ffraud.com
  spf: true
hosts:
- cert_expires: Jan 23 19:32:40 2027 GMT
  host: ffraud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FFraud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FFraud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FFraud
provider_slug: ffraud-com
slug: ffraud-com-domain-security
source_filename: ffraud-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ffraud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 19:32:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ffraud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ffraud-com/security/ffraud-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- IP Lookup
- Email Verification
- Device Fingerprinting
- Open Data
---
