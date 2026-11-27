---
api_specs:
- filename: mailvalid-io-credits-api-openapi.yml
  format: yaml
  label: MailValid Credits API
  slug: mailvalid-io-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailvalid-io/openapi/mailvalid-io-credits-api-openapi.yml
- filename: mailvalid-io-verification-api-openapi.yml
  format: yaml
  label: MailValid Verification API
  slug: mailvalid-io-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailvalid-io/openapi/mailvalid-io-verification-api-openapi.yml
- filename: mailvalid-io-webhooks-api-openapi.yml
  format: yaml
  label: MailValid Webhooks API
  slug: mailvalid-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailvalid-io/openapi/mailvalid-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mailvalid.io
  spf: true
hosts:
- cert_expires: Dec 22 14:31:28 2026 GMT
  host: mailvalid.io
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MailValid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailValid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MailValid
provider_slug: mailvalid-io
slug: mailvalid-io-domain-security
source_filename: mailvalid-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailvalid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 14:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: mailvalid.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mailvalid-io/security/mailvalid-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Verification
- Data Hygiene
- API Service
- Software-as-a-Service
- B2B
---
