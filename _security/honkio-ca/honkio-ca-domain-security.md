---
api_specs:
- filename: honkio-ca-accounts-api-openapi.yml
  format: yaml
  label: honkio-ca Accounts API
  slug: honkio-ca-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-accounts-api-openapi.yml
- filename: honkio-ca-auth-api-openapi.yml
  format: yaml
  label: honkio-ca Auth API
  slug: honkio-ca-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-auth-api-openapi.yml
- filename: honkio-ca-compliance-casl-api-openapi.yml
  format: yaml
  label: honkio-ca Compliance / CASL API
  slug: honkio-ca-compliance-casl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-compliance-casl-api-openapi.yml
- filename: honkio-ca-compliance-dncl-api-openapi.yml
  format: yaml
  label: honkio-ca Compliance / DNCL API
  slug: honkio-ca-compliance-dncl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-compliance-dncl-api-openapi.yml
- filename: honkio-ca-compliance-pipeda-api-openapi.yml
  format: yaml
  label: honkio-ca Compliance / PIPEDA API
  slug: honkio-ca-compliance-pipeda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-compliance-pipeda-api-openapi.yml
- filename: honkio-ca-contact-groups-api-openapi.yml
  format: yaml
  label: honkio-ca Contact Groups API
  slug: honkio-ca-contact-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-contact-groups-api-openapi.yml
- filename: honkio-ca-contacts-api-openapi.yml
  format: yaml
  label: honkio-ca Contacts API
  slug: honkio-ca-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-contacts-api-openapi.yml
- filename: honkio-ca-email-domains-api-openapi.yml
  format: yaml
  label: honkio-ca Email Domains API
  slug: honkio-ca-email-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-email-domains-api-openapi.yml
- filename: honkio-ca-email-suppressions-api-openapi.yml
  format: yaml
  label: honkio-ca Email Suppressions API
  slug: honkio-ca-email-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-email-suppressions-api-openapi.yml
- filename: honkio-ca-email-templates-api-openapi.yml
  format: yaml
  label: honkio-ca Email Templates API
  slug: honkio-ca-email-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-email-templates-api-openapi.yml
- filename: honkio-ca-emails-api-openapi.yml
  format: yaml
  label: honkio-ca Emails API
  slug: honkio-ca-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-emails-api-openapi.yml
- filename: honkio-ca-lists-api-openapi.yml
  format: yaml
  label: honkio-ca Lists API
  slug: honkio-ca-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-lists-api-openapi.yml
- filename: honkio-ca-messages-api-openapi.yml
  format: yaml
  label: honkio-ca Messages API
  slug: honkio-ca-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-messages-api-openapi.yml
- filename: honkio-ca-oauth-api-openapi.yml
  format: yaml
  label: honkio-ca OAuth API
  slug: honkio-ca-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-oauth-api-openapi.yml
- filename: honkio-ca-phone-numbers-api-openapi.yml
  format: yaml
  label: honkio-ca Phone Numbers API
  slug: honkio-ca-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-phone-numbers-api-openapi.yml
- filename: honkio-ca-pricing-api-openapi.yml
  format: yaml
  label: honkio-ca Pricing API
  slug: honkio-ca-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-pricing-api-openapi.yml
- filename: honkio-ca-verify-api-openapi.yml
  format: yaml
  label: honkio-ca Verify API
  slug: honkio-ca-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-verify-api-openapi.yml
- filename: honkio-ca-webhooks-api-openapi.yml
  format: yaml
  label: honkio-ca Webhooks API
  slug: honkio-ca-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/honkio-ca/openapi/honkio-ca-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: honkio.ca
  spf: false
hosts:
- cert_expires: Dec 31 16:15:50 2026 GMT
  host: honkio.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Honkio Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for honkio-ca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: honkio-ca
provider_slug: honkio-ca
slug: honkio-ca-domain-security
source_filename: honkio-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honkio.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 16:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: honkio.ca\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/honkio-ca/security/honkio-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SMS
- Email
- Canada
- CASL
- PIPEDA
- Company
---
