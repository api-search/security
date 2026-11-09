---
api_specs:
- filename: mailfloss-account-api-openapi.yml
  format: yaml
  label: mailfloss Account API
  slug: mailfloss-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-account-api-openapi.yml
- filename: mailfloss-batch-api-openapi.yml
  format: yaml
  label: mailfloss Batch API
  slug: mailfloss-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-batch-api-openapi.yml
- filename: mailfloss-integrations-api-openapi.yml
  format: yaml
  label: mailfloss Integrations API
  slug: mailfloss-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-integrations-api-openapi.yml
- filename: mailfloss-privacy-api-openapi.yml
  format: yaml
  label: mailfloss Privacy API
  slug: mailfloss-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-privacy-api-openapi.yml
- filename: mailfloss-reports-api-openapi.yml
  format: yaml
  label: mailfloss Reports API
  slug: mailfloss-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-reports-api-openapi.yml
- filename: mailfloss-team-api-openapi.yml
  format: yaml
  label: mailfloss Team API
  slug: mailfloss-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-team-api-openapi.yml
- filename: mailfloss-verification-api-openapi.yml
  format: yaml
  label: mailfloss Verification API
  slug: mailfloss-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-verification-api-openapi.yml
- filename: mailfloss-webhooks-api-openapi.yml
  format: yaml
  label: mailfloss Webhooks API
  slug: mailfloss-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfloss/openapi/mailfloss-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mailfloss.com
  spf: true
hosts:
- cert_expires: Jan  1 09:14:01 2027 GMT
  host: mailfloss.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailfloss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailfloss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mailfloss
provider_slug: mailfloss
slug: mailfloss-domain-security
source_filename: mailfloss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailfloss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 09:14:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailfloss.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mailfloss/security/mailfloss-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Verification
- Marketing
- Software-as-a-Service
- Automation
- Deliverability
---
