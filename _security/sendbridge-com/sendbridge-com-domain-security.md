---
api_specs:
- filename: sendbridge-com-account-api-openapi.yml
  format: yaml
  label: SendBridge Account API
  slug: sendbridge-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-account-api-openapi.yml
- filename: sendbridge-com-dmarc-api-openapi.yml
  format: yaml
  label: SendBridge DMARC API
  slug: sendbridge-com-dmarc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-dmarc-api-openapi.yml
- filename: sendbridge-com-mail-tester-api-openapi.yml
  format: yaml
  label: SendBridge Mail Tester API
  slug: sendbridge-com-mail-tester-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-mail-tester-api-openapi.yml
- filename: sendbridge-com-validation-api-openapi.yml
  format: yaml
  label: SendBridge Validation API
  slug: sendbridge-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-validation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sendbridge.com
  spf: true
hosts:
- cert_expires: Dec 25 17:45:40 2026 GMT
  host: sendbridge.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sendbridge Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SendBridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SendBridge
provider_slug: sendbridge-com
slug: sendbridge-com-domain-security
source_filename: sendbridge-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendbridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 17:45:40 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: sendbridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sendbridge-com/security/sendbridge-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- email
- verification
- api
- deliverability
- validation
- marketing
- service
---
