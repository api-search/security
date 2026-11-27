---
api_specs:
- filename: mailtester-com-agent-gateway-api-openapi.yml
  format: yaml
  label: MailTester Agent Gateway API
  slug: mailtester-com-agent-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtester-com/openapi/mailtester-com-agent-gateway-api-openapi.yml
- filename: mailtester-com-credits-api-openapi.yml
  format: yaml
  label: MailTester Credits API
  slug: mailtester-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtester-com/openapi/mailtester-com-credits-api-openapi.yml
- filename: mailtester-com-verify-api-openapi.yml
  format: yaml
  label: MailTester Verify API
  slug: mailtester-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtester-com/openapi/mailtester-com-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mailtester.com
  spf: true
hosts:
- cert_expires: Jan 13 01:36:07 2027 GMT
  host: mailtester.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MailTester Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailTester, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MailTester
provider_slug: mailtester-com
slug: mailtester-com-domain-security
source_filename: mailtester-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailtester.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 01:36:07 2027 GMT\n  hsts: false\ndomains:\n- domain: mailtester.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mailtester-com/security/mailtester-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Email Verification
- Deliverability Testing
- List Cleaning
- Marketing Tools
---
