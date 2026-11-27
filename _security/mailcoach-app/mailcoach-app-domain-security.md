---
api_specs:
- filename: mailcoach-app-automation-mails-api-openapi.yml
  format: yaml
  label: Mailcoach Automation Mails API
  slug: mailcoach-app-automation-mails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-automation-mails-api-openapi.yml
- filename: mailcoach-app-automations-api-openapi.yml
  format: yaml
  label: Mailcoach Automations API
  slug: mailcoach-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-automations-api-openapi.yml
- filename: mailcoach-app-campaign-statistics-api-openapi.yml
  format: yaml
  label: Mailcoach Campaign Statistics API
  slug: mailcoach-app-campaign-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-campaign-statistics-api-openapi.yml
- filename: mailcoach-app-campaigns-api-openapi.yml
  format: yaml
  label: Mailcoach Campaigns API
  slug: mailcoach-app-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-campaigns-api-openapi.yml
- filename: mailcoach-app-links-api-openapi.yml
  format: yaml
  label: Mailcoach Links API
  slug: mailcoach-app-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-links-api-openapi.yml
- filename: mailcoach-app-lists-api-openapi.yml
  format: yaml
  label: Mailcoach Lists API
  slug: mailcoach-app-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-lists-api-openapi.yml
- filename: mailcoach-app-segments-api-openapi.yml
  format: yaml
  label: Mailcoach Segments API
  slug: mailcoach-app-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-segments-api-openapi.yml
- filename: mailcoach-app-sends-api-openapi.yml
  format: yaml
  label: Mailcoach Sends API
  slug: mailcoach-app-sends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-sends-api-openapi.yml
- filename: mailcoach-app-subscriber-imports-api-openapi.yml
  format: yaml
  label: Mailcoach Subscriber Imports API
  slug: mailcoach-app-subscriber-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-subscriber-imports-api-openapi.yml
- filename: mailcoach-app-subscribers-api-openapi.yml
  format: yaml
  label: Mailcoach Subscribers API
  slug: mailcoach-app-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-subscribers-api-openapi.yml
- filename: mailcoach-app-suppressions-api-openapi.yml
  format: yaml
  label: Mailcoach Suppressions API
  slug: mailcoach-app-suppressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-suppressions-api-openapi.yml
- filename: mailcoach-app-tags-api-openapi.yml
  format: yaml
  label: Mailcoach Tags API
  slug: mailcoach-app-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-tags-api-openapi.yml
- filename: mailcoach-app-templates-api-openapi.yml
  format: yaml
  label: Mailcoach Templates API
  slug: mailcoach-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-templates-api-openapi.yml
- filename: mailcoach-app-transactional-mails-api-openapi.yml
  format: yaml
  label: Mailcoach Transactional Mails API
  slug: mailcoach-app-transactional-mails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-transactional-mails-api-openapi.yml
- filename: mailcoach-app-uploads-api-openapi.yml
  format: yaml
  label: Mailcoach Uploads API
  slug: mailcoach-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcoach-app/openapi/mailcoach-app-uploads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mailcoach.app
  spf: true
hosts:
- cert_expires: Jan 27 19:17:20 2027 GMT
  host: mailcoach.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailcoach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailcoach, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mailcoach
provider_slug: mailcoach-app
slug: mailcoach-app-domain-security
source_filename: mailcoach-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailcoach.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:17:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailcoach.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mailcoach-app/security/mailcoach-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Marketing
- GDPR
---
