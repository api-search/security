---
api_specs:
- filename: elocuenti-com-account-api-openapi.yml
  format: yaml
  label: Elocuenti Account API
  slug: elocuenti-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-account-api-openapi.yml
- filename: elocuenti-com-audit-api-openapi.yml
  format: yaml
  label: Elocuenti Audit API
  slug: elocuenti-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-audit-api-openapi.yml
- filename: elocuenti-com-automations-api-openapi.yml
  format: yaml
  label: Elocuenti Automations API
  slug: elocuenti-com-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-automations-api-openapi.yml
- filename: elocuenti-com-calls-api-openapi.yml
  format: yaml
  label: Elocuenti Calls API
  slug: elocuenti-com-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-calls-api-openapi.yml
- filename: elocuenti-com-carts-api-openapi.yml
  format: yaml
  label: Elocuenti Carts API
  slug: elocuenti-com-carts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-carts-api-openapi.yml
- filename: elocuenti-com-contacts-api-openapi.yml
  format: yaml
  label: Elocuenti Contacts API
  slug: elocuenti-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-contacts-api-openapi.yml
- filename: elocuenti-com-conversations-api-openapi.yml
  format: yaml
  label: Elocuenti Conversations API
  slug: elocuenti-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-conversations-api-openapi.yml
- filename: elocuenti-com-events-api-openapi.yml
  format: yaml
  label: Elocuenti Events API
  slug: elocuenti-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-events-api-openapi.yml
- filename: elocuenti-com-feedback-api-openapi.yml
  format: yaml
  label: Elocuenti Feedback API
  slug: elocuenti-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-feedback-api-openapi.yml
- filename: elocuenti-com-knowledge-api-openapi.yml
  format: yaml
  label: Elocuenti Knowledge API
  slug: elocuenti-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-knowledge-api-openapi.yml
- filename: elocuenti-com-messages-api-openapi.yml
  format: yaml
  label: Elocuenti Messages API
  slug: elocuenti-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-messages-api-openapi.yml
- filename: elocuenti-com-orders-api-openapi.yml
  format: yaml
  label: Elocuenti Orders API
  slug: elocuenti-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-orders-api-openapi.yml
- filename: elocuenti-com-payments-api-api-openapi.yml
  format: yaml
  label: Elocuenti Payments API
  slug: elocuenti-com-payments-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-payments-api-api-openapi.yml
- filename: elocuenti-com-pipelines-api-openapi.yml
  format: yaml
  label: Elocuenti Pipelines API
  slug: elocuenti-com-pipelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-pipelines-api-openapi.yml
- filename: elocuenti-com-templates-api-openapi.yml
  format: yaml
  label: Elocuenti Templates API
  slug: elocuenti-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-templates-api-openapi.yml
- filename: elocuenti-com-webhooks-api-openapi.yml
  format: yaml
  label: Elocuenti Webhooks API
  slug: elocuenti-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elocuenti-com/openapi/elocuenti-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elocuenti.com
  spf: true
hosts:
- cert_expires: Jan 21 10:04:16 2027 GMT
  host: elocuenti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elocuenti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elocuenti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elocuenti
provider_slug: elocuenti-com
slug: elocuenti-com-domain-security
source_filename: elocuenti-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elocuenti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 10:04:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: elocuenti.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elocuenti-com/security/elocuenti-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Omnichannel
- Automation
- Integration
---
