---
api_specs:
- filename: hail-so-agents-api-openapi.yml
  format: yaml
  label: Hail Agents API
  slug: hail-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-agents-api-openapi.yml
- filename: hail-so-calls-api-openapi.yml
  format: yaml
  label: Hail Calls API
  slug: hail-so-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-calls-api-openapi.yml
- filename: hail-so-contacts-api-openapi.yml
  format: yaml
  label: Hail Contacts API
  slug: hail-so-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-contacts-api-openapi.yml
- filename: hail-so-email-attachments-api-openapi.yml
  format: yaml
  label: Hail Email Attachments API
  slug: hail-so-email-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-email-attachments-api-openapi.yml
- filename: hail-so-email-domains-api-openapi.yml
  format: yaml
  label: Hail Email Domains API
  slug: hail-so-email-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-email-domains-api-openapi.yml
- filename: hail-so-emails-api-openapi.yml
  format: yaml
  label: Hail Emails API
  slug: hail-so-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-emails-api-openapi.yml
- filename: hail-so-events-api-openapi.yml
  format: yaml
  label: Hail Events API
  slug: hail-so-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-events-api-openapi.yml
- filename: hail-so-forward-targets-api-openapi.yml
  format: yaml
  label: Hail Forward Targets API
  slug: hail-so-forward-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-forward-targets-api-openapi.yml
- filename: hail-so-healthz-api-openapi.yml
  format: yaml
  label: Hail Healthz API
  slug: hail-so-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-healthz-api-openapi.yml
- filename: hail-so-numbers-api-openapi.yml
  format: yaml
  label: Hail Numbers API
  slug: hail-so-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-numbers-api-openapi.yml
- filename: hail-so-providers-api-openapi.yml
  format: yaml
  label: Hail Providers API
  slug: hail-so-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-providers-api-openapi.yml
- filename: hail-so-sms-api-openapi.yml
  format: yaml
  label: Hail Sms API
  slug: hail-so-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-sms-api-openapi.yml
- filename: hail-so-unsubscribe-api-openapi.yml
  format: yaml
  label: Hail Unsubscribe API
  slug: hail-so-unsubscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-unsubscribe-api-openapi.yml
- filename: hail-so-uploads-api-openapi.yml
  format: yaml
  label: Hail Uploads API
  slug: hail-so-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-uploads-api-openapi.yml
- filename: hail-so-verifications-api-openapi.yml
  format: yaml
  label: Hail Verifications API
  slug: hail-so-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-verifications-api-openapi.yml
- filename: hail-so-webhooks-api-openapi.yml
  format: yaml
  label: Hail Webhooks API
  slug: hail-so-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-webhooks-api-openapi.yml
- filename: hail-so-whoami-api-openapi.yml
  format: yaml
  label: Hail Whoami API
  slug: hail-so-whoami-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hail-so/openapi/hail-so-whoami-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hail.so
  spf: true
hosts:
- cert_expires: Feb  4 07:28:04 2027 GMT
  host: hail.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hail
provider_slug: hail-so
slug: hail-so-domain-security
source_filename: hail-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hail.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 07:28:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hail.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hail-so/security/hail-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Communications
- Phone
- SMS
- Email
---
