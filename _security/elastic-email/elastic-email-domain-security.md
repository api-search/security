---
api_specs:
- filename: elastic-email-elastic-email-api-api-openapi.yml
  format: yaml
  label: Elastic Email Elastic Email API
  slug: elastic-email-elastic-email-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-email/refs/heads/main/openapi/elastic-email-elastic-email-api-api-openapi.yml
- filename: elastic-email-emails-api-openapi.yml
  format: yaml
  label: Elastic Email Emails API
  slug: elastic-email-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-email/refs/heads/main/openapi/elastic-email-emails-api-openapi.yml
- filename: elastic-email-hooks-api-openapi.yml
  format: yaml
  label: Elastic Email Hooks API
  slug: elastic-email-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-email/refs/heads/main/openapi/elastic-email-hooks-api-openapi.yml
- filename: elastic-email-webhook-api-openapi.yml
  format: yaml
  label: Elastic Email Webhook API
  slug: elastic-email-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elastic-email/refs/heads/main/openapi/elastic-email-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elasticemail.com
  spf: true
hosts:
- cert_expires: Dec 20 07:05:52 2026 GMT
  host: elasticemail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elastic Email Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elastic Email, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elastic Email
provider_slug: elastic-email
slug: elastic-email-domain-security
source_filename: elastic-email-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elasticemail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 07:05:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elasticemail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elastic-email/refs/heads/main/security/elastic-email-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Marketing
- Software-as-a-Service
---
